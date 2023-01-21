# I-Bond-Interest-Rate-History
Treasury Direct I bond interest rate history data in Excel and csv formats.

This was created using the Treasury Direct I Bond interest rate history chart at https://www.treasurydirect.gov/savings-bonds/i-bonds/i-bonds-interest-rates/

## About The Files ##
+ The csv file contains the data from the Treasury Direct rate chart.  The last row contains the semiannual inflation rates, like the original chart.
+ The Excel version contains the following customizations:
  - Moved the semiannual inflation rate row to the top
  - Enabled freeze panes in cell C3 to keep the top and left headings visible while scrolling

## Instructions to extract and convert the data using [Notepad++](https://notepad-plus-plus.org/) and Excel ##
1. Open the I Bond rate history pdf file https://www.treasurydirect.gov/files/savings-bonds/i-bond-rate-chart.pdf
2. Copy the entire rate history table.  *It's ok if you select some of the text above and below the table because you can remove it in Notepad++.*
3. Open Notepad++
4. Paste the data into a new Notepad++ document
5. Click View > Show Symbol and enable Show All Characters
6. Delete any extra text above and below the table.  Keep the header row beginning with Issue
7. Click Search > Replace
8. In the Replace window:
   1. Put a <kbd>space</kbd> in the Find field
   2. Enter \t in the Replace field
   3. Set Search Mode to Extended
   4. Click Replace All
   5. In the Replace window, change the find field from a <kbd>space</kbd> to \t-\t  *Make sure you remove the <kbd>space</kbd> character.*
   6. Change the replace field to <kbd>space</kbd>-<kbd>space</kbd>
   7. Click Replace All
   8. Close the Replace window
9. On the first line, replace the <kbd>tab</kbd> after Issue with a <kbd>space</kbd>.  Add a <kbd>tab</kbd> after Issue Date.  Delete the new line character(s).
10. Delete the new line character(s) after Fixed.  Insert a <kbd>space</kbd> between Fixed and Rate
11. Scroll to the last line
12. Replace the <kbd>tab</kbd> after Semiannual with a <kbd>space</kbd>
13. Delete the new line character(s).
14. Insert a <kbd>space</kbd> between Inflation and Rate
15. Insert a second <kbd>tab</kbd> after Rate
16. Select all of the text and copy it
17. Paste the text into a new Excel workbook
