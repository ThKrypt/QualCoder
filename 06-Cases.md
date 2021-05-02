# Manage cases

Cases are useful for seeing text and images linked to a particular circumstance or person and for assigning attributes such as age and gender to interview participants. You can add a memo of notes to each case and rename a case by double-clicking on a case name.


A table lists the cases and their attributes. On the right had side the text of a case is displayed. The number of files associated with a case is shown. Click on the files cell in the table to add or changes files associated with a case. This displays the case file manager dialog, described below.

When a survey is imported, each survey row is assigned to a case. The case name is the unique identifier in the first column of the csv or Excel spreadsheet. Large surveys (e.g. 1000 or more rows) can take a long time to import as cases take some time to create.

![Manage cases tab](https://qualcoder.files.wordpress.com/2021/05/cases.png?resize=450%2C450)

Practical example: Add the three students (or cases) by clicking the Add case icon. Name each student: ID1, ID2 and ID3.

## Case file manager

Now, add each student’s file to each student. Click on the cell in the Files column for case ID3 for example. This opens the _case file manager dialog_. Alternatively, click on the documents icon which will also open the case file manager.

![Case File Manager](https://qualcoder.files.wordpress.com/2020/08/case-file-manager.png)

In the _case file manager_, click on a case, say ID3, then click  Add selected files to case button. Select one or more files in the files list. Add the files to the case. For  example add the miguel-henriques.jpg to ID3. You can remove files and view the files associated with the case. You will see file text will be underlined in red which indicates this text is associated with this case.

Now open the transcript.txt file. Notice the transcript begins with a student id inside square brackets [ ].

Try automatically assigning text to ID1 by selecting case ID1 then clicking the Auto assign file text button. You will be asked which file or files to assign the case to. Select transcript.txt from the list. Next you need to enter the start and end marks. The start mark will be ‘[id1]’ and the end mark will be ‘[‘, note this is case sensitive so that is why you use the lower case here.

![Auto-assign start and end marks](https://qualcoder.files.wordpress.com/2019/01/automarking_case.png?w=443&h=232)

Now select the case ID1 and see the assigned text.

You can also select a case, manually highlight text, and right-click to mark – or assign -the text to the selected case.

## Importing cases

You can import attributes from a CSV or XLSX file. The first row must contain the attribute headings. The first column must contain matching case names (for this example: ID1, ID2, ID3). Note that this is case sensitive. Open the cases.csv file in the Examples folder to see how it is laid out.

For this example – delete all the cases shown. Then, import the attributes from the cases.csv file through the Import Attributes dialog. You will again need to link the files and file text to each case.