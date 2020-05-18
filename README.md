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
