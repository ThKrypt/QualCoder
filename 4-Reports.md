# Coding Reports

This dialog gives a list of coded text based on your selections. One or more codes need to be selected and one or both of coder 1 and coder 2 need to be selected. The Search button will present the results. If a category is selected all codes in that category are also selected. Multiple categories can be selected using the mouse and the ‘ctrl’ button. Codes and categories can be sorted to help find the codes of interest.

Codings can be narrowed down by using the File selection Case selection or Attribute selection buttons. Only codings within the selected files or cases will be presented. If text is entered into the Search text field, only codings which contain the matching text will be presented. Codings can also be narrowed down to case selections using the Case selection button. Note that when case selections are used, file selections are ignored. Also when file selections are used, case selections are ignored.

The Search Text box also limits the reported codings. The search text looks for any codings in text that contain the search text. The search text also looks for matching text in memos for coded image areas and coded audio/video segments. The search text function must be used in combination with File selection, Case selection or Attribute selection.

The Attribute selection button opens a dialog window where you can select attributes for files and cases, for example: only interview files for people aged > 60.

![Attribute selection](https://qualcoder.files.wordpress.com/2019/02/attribute_selection.png)

If you are creating a report based on Case selection, then the code tree pane is hidden. Instead two panes are shown. The left pane shows the codings in a list, the right pane shows a matrix with one case on each row and top-level categories in each column, shown as below:

![Case report showing three panes](https://qualcoder.files.wordpress.com/2019/08/report_panes-1.png)

Each of the three panes can be widened or narrowed by dragging with the mouse on the bar that splits each section.
Reports can be exported to text, open document (ODT), html or csv files. Currently case matrices are not able to be exported.

##  Coding Comparison
This option shows the similarities and differences between two coders. Select two coders and click the run comparisons button. The statistics created here are only for coded text, not coded media files. For each code:

Agreement % shows agreement for a combination of coded and non-coded text characters.

A and B % shows agreement for the only the coded text characters divided by the total characters in the text.

Not A and Not B % shows the total of the uncoded text divided by the total characters in the text.

Disagree % shows the percentage of all the coded and non-coded text that did not match between coders. It is the same as 100 – the Agree %.

Cohen’s Kappa is calculated based on the information in Wikipedia https://en.wikipedia.org/wiki/Cohen%27s_kappa

![Coder comparison](https://qualcoder.files.wordpress.com/2019/01/coder-comparison.png)

#  SQL Statements Dialog

This dialog contains three panes. The top pane is where SQL statements are entered and the bottom pane contains the results of queries. The left pane contains tables and field names. Double-clicking on a field name adds it to the SQL statement. Results can be exported to a text file. If you are not familiar with SQL take care as you will be able to update and delete the data as well as select data. Note: Some Unicode symbols are not converted to plain text and are ignored.

Most table fields are text. The following fields are integer: anid, avid, attrid, caseid,catid, cid, fid, id, imid, jid, pos0,pos1, x1, y1, width, height.

#  Multiple dialog windows

It is possible to have multiple dialog windows open. This is useful if you have run a report, or have a file open for coding, and you want to enter your thoughts into a journal entry. **However there are some limitations**.
 
Some dialog windows are priority windows, so swapping between windows will not be possible, these restricted windows are: Management of files, cases or attributes, survey import and confirmation dialogs (e.g. confirm delete). 

The second limitation is that changes in one dialog will not be reflected in the other dialogs. An example here is adding a code in a coding dialog, the added code will not be shown in other coding or reports windows. If you do make changes to highlighting and codes and categories, it is recommended to close and then re-open the other dialog window that you need. This is to ensure that any changes made show up in the other dialog windows. Similarly, highlighting text on the same file in two opened dialog will not be reflected in the other window. A warning, if you have the same journal entry open in two windows, the last window that is closed will be the entry that is saved.

A programming quirk is if you open a dialog (e.g. manage files dialog) close it,then immediately try to re-open it. The dialog will not be visible. To get around this, open a different dialog, close it, then open the manage files dialog again.

![Multiple dialogs](https://qualcoder.files.wordpress.com/2019/08/multiple_dialogs.png)

