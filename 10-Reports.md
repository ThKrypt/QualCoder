# Reports menu options
* Coding reports
* Coding comparison
* Code frequencies
* View graph
* Code relations
* SQL statements (run SQL queries)

# Coding Reports

This dialog gives a list of coded text based on your selections. One or more codes need to be selected. If a category is selected all codes in that category are also selected. Multiple categories can be selected using the mouse and the ‘ctrl’ button. 

The Search button (Button containing cogs) will present the results.

![Coding report in dark mode](https://qualcoder.files.wordpress.com/2021/05/coding_report-1.png?resize=760%2C500)

_Coding report showing results of coded text and images, in dark mode_

Coding results can be narrowed down by using the File selection, Case selection or Attribute selection buttons. Only codings within the selected files or cases will be presented. When case selections are used, file selections are ignored. Also when file selections are used, case selections are ignored. 

If text is entered into the Search text field, only codings which contain the matching text will be presented. 
The search text also looks for matching text in memos for coded image areas and coded audio/video segments. The search text function must be used in combination with File selection, Case selection or Attribute selection.

** Important coded text, images, segments
There is a tick box to select only the Important codings. This is useful for quickly finding those important exemplars that you may use in a written report.

## Attribute selection in reports

The Attribute selection button opens a dialog window where you can select attributes for files and cases, for example: only interview files for people aged > 60.

![Attribute selection](https://qualcoder.files.wordpress.com/2019/02/attribute_selection.png)

## Case selection in reports
If you are creating a report and selecting cases, then the code tree pane is narrowed. Three panes are shown. The left pane shows the codings in a list, the middle pane shows the highlighted codes, the right pane shows a matrix with one case on each row in columns. The column types can be codes, categories, or top-level categories.

Each of the three panes can be widened or narrowed by dragging with the mouse on the bar that splits each section.
Reports can be exported to text, open document (ODT), html or csv files. Currently, case matrices are not able to be exported.
The second pane with show all the results in a list allows you to view the coded portion in context of the original text file, image, audio or video. To do this, click on the row of text that begins with [VIEW].

![Case selection in reports](https://qualcoder.files.wordpress.com/2021/05/coding_report_categories.png?resize=760%2C500)

_When cases are selected, another pane is displayed showing a table of cases (in rows) and categories or codes in columns_

* Shortcut H. Pressing h will hide and unhide the top controls section of the window.

## Other functions

* Check box to add summary statistics to the report.
* Matrix options. So have codes/categories by file or by case. The matrix can be transposed, using the check box.
* Check box for coding in context for coded text segments. This shows the surrounding 250 characters of text to help put the coded section in context in the report. The coded text segment is shown in bold.

#  Coding Comparison
This option shows the overall similarities and differences between two coders across all text files. Select two coders and click the run comparisons button. The statistics created here are only for coded text, not coded image nor media files. 

For each code:

Agreement % shows agreement for a combination of coded and non-coded text characters.

A and B % shows agreement for the only the coded text characters divided by the total characters in the text.

Not A and Not B % shows the total of the uncoded text divided by the total characters in the text.

Disagree % shows the percentage of all the coded and non-coded text that did not match between coders. It is the same as 100 – the Agree %.

Agree coded only % shows the percentage of all the dual coded text divided by single plus dual coded text. (In version 3.1 +)

Cohen’s Kappa is calculated based on the information in Wikipedia https://en.wikipedia.org/wiki/Cohen%27s_kappa

![Coder comparison](https://qualcoder.files.wordpress.com/2019/01/coder-comparison.png)

#  Coding Comparison by file

This option shows the overall similarities and differences between two coders in ONE selected file. Select one file, one code and two coders. Then click the run comparisons button. The statistics and comparisons for audio/video coded segments are in development. 
Overall agreement, disagreement and Cohens Kappa are calculated for text and images. An image file is displayed in a separate window showing the two coders selections in yellow or blue boxed areas. Mouse hover provides additional information.

# Code frequencies

This window shows all the codes and categories and the frequency of use for each coder. Code frequencies can be selected for specific files.

![Code frequencies report](https://qualcoder.files.wordpress.com/2021/05/code_frequencies.png?resize=450%2C700)

#  Graph

A graph of categories and codes is displayed. You can choose all or selected categories. 
Each code or category can be moved around by clicking near the edge of the box and dragging it around. Right-clicking in a code gives a menu of options such as displaying the memo, or displaying all the case or file text that has been coded with the selected code.

In the 3.1 version (not yet released) you can add files, cases, codings, coding memos and free text items to this graph. Graphs can also be saved, loaded and deleted. This means that the graph can be used for coding maps, or concept or mind maps.

![Node graph](https://qualcoder.files.wordpress.com/2020/08/node-graph.png)


# Code relations

This dialog shows the relations between two or more codes. This can only be applied to text files. 
The relations are:

* Proximity – Two codes do not overlap. The distance in  number of characters is shown.
* Overlap – Two codes partially overlap. The lowest and highest character positions of the combination are shown. The union of the overlapping section is shown in character positions.
* Inclusion – One code is included within another code. The lowest and highest character positions of the combination are shown. The union of the overlapping section is shown in character positions.
* Exact – Both codes match in their start and end positions. The lowest and highest character positions of the combination are shown. The union of the overlapping section is shown in character positions.

A csv file can be exported.

# File Summary

Click on a file to get a summary of that file. It describes media metadata, characters and word frequency. Attributes. It summarises the count of codes for that file. For text codings is summarises the average text length. For image codings it summarises the average pixel area. For audio/video codings it summarises the average segment length.

# Code Summary

Click on a code to get a summary of that code. The coders who have used the code. The number of codings in text, image and audio/video media. For text codings is summarises the average text length and the most common words. For image codings it summarises the average pixel area. For audio/video codings it summarises the average segment length.

![Code summary](https://qualcoder.files.wordpress.com/2021/05/code_summary_report.png?resize=700%2C500)

# Charts

Charts are displayed in the default web browser.

Pie, Bar, Sunburst and Treemap charts can be created.

Heatmaps of files or cases against codes can be created. These are limited to 40 rows and columns for quicker rendering and better visibility.

#  SQL Statements (run SQL queries)

This window contains three panes. The top pane is where SQL statements are entered and the bottom pane contains the results of queries. The left pane contains tables and field names. Double-clicking on a field name adds it to the SQL statement. Results can be exported to a delimited file. If you are not familiar with SQL take care as you will be able to update and delete the data as well as select data. Note: Some Unicode symbols are not converted to plain text and are ignored.

There are several prepared join statements listed:
* Case text
* Codes fileid and coded text
* Get coding table - an implementation of an RQDA function that returns the code name, table, text length and text start and end positions.
* Coded text with each case

Most table fields are text. The following fields are integer: anid, avid, attrid, caseid,catid, cid, fid, id, imid, jid, pos0,pos1, x1, y1, width, height.

Right-click in the results table for filtering options.

Right click in the SQL window give you various options such as select all, copy, paste.

![SQL dialog](https://qualcoder.files.wordpress.com/2019/01/sql-statements2.png)







