# stock-analysis
Stock Analysis
---
### Optimize stock analysis code for performance
1. Rewrote the module 2 code for performance
2. The original code (AllStockAnalysis() went through each ticker symbol at a time through all the rows, i.e 3012 * 12 times.
3. The new code (modified the AllStockAnalysis() to module 3 : AllStockAnalysisRefactored())goes through the rows in a sheet once (3012) and collects/compute the data with array of variables for volume, starting price , ending price  per ticker
4. Dispalys the results from these arrays in another sheet by using for loops
5. This way, active sheets to do not need to be constantly swapping between stock sheets and  analysis sheet.
6. Go through only once through the sheet of rows to get what we need
7. Assumption, the sheet is already ready with ticker symbols sorted so that we can determine when we transition from one ticker to another. 
8. We created array of variable (array length = number of stocks), for volume, strating price, ending price.
9. Ask the user for the sheet to analyze (i.e year)
10. Initialize the variables and stock tickers we want to analyze
11. Go through the rows in the selected sheet (using for loops) to accumulate volume for each ticker.
12. When the ticker symbol changes, capture the starting price , i.e pervious symbol is different from current one. Happens to be true for the second row also.
13. When the next row tciker symbol is differnet, the current ticker price is the ending price, happens to be true for the last ticker also.
14. loop through the tickers, volume, starting price , ending price arrays to display it in the All Stock Analysis sheet.
15. Buttons in the all stock analysis sheet to clear and also run the analysis,
