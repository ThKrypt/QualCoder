# Reports menu options
* Coding reports
* Coding comparison
* Code frequencies
* View graph
* Code relations
* SQL dialog

# Coding Reports

This dialog gives a list of coded text based on your selections. One or more codes need to be selected. If a category is selected all codes in that category are also selected. Multiple categories can be selected using the mouse and the ‘ctrl’ button. 

The Search button will present the results.

Coding results can be narrowed down by using the File selection, Case selection or Attribute selection buttons. Only codings within the selected files or cases will be presented. When case selections are used, file selections are ignored. Also when file selections are used, case selections are ignored. 

If text is entered into the Search text field, only codings which contain the matching text will be presented. 
The search text also looks for matching text in memos for coded image areas and coded audio/video segments. The search text function must be used in combination with File selection, Case selection or Attribute selection.

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

# Code frequencies

This window shows all the codes and categories and the frequency of use for each coder 

#  Node graph

A graph of categories and codes is displayed. There are several options to change what is shown – such as Black and White, All or selected categories.

Each code or category can be moved around by clicking near the edge of the box and dragging it around. Clicking on the text allows you to temporarily change the code or category wording. Right-clicking in a code gives a menu of options such as displaying the memo, or displaying all the case or file text that has been coded with the selected code.

![Node graph](https://qualcoder.files.wordpress.com/2019/01/node-graph.png)

# Code relations

This dialog show the relations between two or more codes. This can only be applied to text files. 
The relations are:

* Proximity – Two codes do not overlap. The distance in  number of characters is shown.
* Overlap – Two codes partially overlap. The lowest and highest character positions of the combination are shown. The union of the overlapping section is shown in character positions.
* Inclusion – One code is included within another code. The lowest and highest character positions of the combination are shown. The union of the overlapping section is shown in character positions.
* Exact – Both codes match in their start and end positions. The lowest and highest character positions of the combination are shown. The union of the overlapping section is shown in character positions.

A csv file can be exported.

#  SQL Dialog

This dialog contains three panes. The top pane is where SQL statements are entered and the bottom pane contains the results of queries. The left pane contains tables and field names. Double-clicking on a field name adds it to the SQL statement. Results can be exported to a text file. If you are not familiar with SQL take care as you will be able to update and delete the data as well as select data. Note: Some Unicode symbols are not converted to plain text and are ignored.

Most table fields are text. The following fields are integer: anid, avid, attrid, caseid,catid, cid, fid, id, imid, jid, pos0,pos1, x1, y1, width, height.


#  Codebook

A codebook is a list of your codes. Each code memo should detail the reasons for the purpose of each code. The codebook can be exported to a text file. The codebook also shows the frequency of the codes used (from all coders). Example codebook output is shown below. As codes and categories are put in a tree like structure the double minus ‘–‘ indicates the subordinate codes and categories within a category.



#  Multiple dialog windows

It is possible to have multiple dialog windows open. This is useful if you have run a report, or have a file open for coding, and you want to enter your thoughts into a journal entry. **However there are some limitations**.
 
Some dialog windows are priority windows, so swapping between windows will not be possible, these restricted windows are: Management of files, cases or attributes, survey import and confirmation dialogs (e.g. confirm delete). 

The second limitation is that changes in one dialog will not be reflected in the other dialogs. An example here is adding a code in a coding dialog, the added code will not be shown in other coding or reports windows. If you do make changes to highlighting and codes and categories, it is recommended to close and then re-open the other dialog window that you need. This is to ensure that any changes made show up in the other dialog windows.



