# autofill_formulas_2
GOOGLE APP SCRIPT (Sheets): Enter formulas in required cells automatically. (Code for repetitive task) (For complex operations)

Explanation of the code:

> Function Definition: The function `autofill_formulas_1()` is defined to autofill formulas into specific cells in a Google Spreadsheet.

> Active Spreadsheet and Sheet Selection:  
 - The function targets the active spreadsheet and selects the sheet named `'black_friday'`.

> Outer Loop (20 iterations):  
 - A loop runs 20 times, starting with row 51, incrementing by 7 for each iteration (`targetRow`).
 - A corresponding source row starts from row 44 and increments by 6 (`sourceRow`).

> Inner Loop (Columns D to I):  
 - Another loop iterates over columns D to I (columns 4 to 9).

> Formula Creation:  
 - For each column, a formula is generated using the `getRange()` method on the columns U to Z (columns 21 to 26) in the first row.
 - The formula references the corresponding source row, and the column letters are adjusted dynamically using `replace()` to remove row numbers.

> Formula Application:  
 - The formula is then set in the corresponding target cell (identified by `targetRow` and `col`).

> Outcome:  
 - This process autofills the cells from row 51 onward, applying formulas in columns D to I based on the structure of cells in columns U to Z.
