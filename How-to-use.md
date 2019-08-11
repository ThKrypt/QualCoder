There are a few sample files in the Examples folder. These can be used to test importing files of different document formats and of importing an image. There are also example files to test importing case attributes, and for importing a survey.

#  Create a new project

Create a new project under the ‘Project’ menu, call it test. The project wil be saved as test.qda. Test.qda is actually a folder containing subfolders which hold the database and other files. Additionally, in your home folder QualCoder will create a .qualcoder folder with a QualCoder.log file for logging events, including hopefully all software errors and exceptions and a QualCoder_settings.txt file which will contain the current coder’s name, preferred fonts and a preferred working directory.

Under the Project menu click on Project memo. This is a memo about your project. Type “A test QDA project” and click the OK button.

The main window displays various changes that are made when using QualCoder. You will notice the main window displays the following, with a menu bar at the top:

![main screen](https://qualcoder.files.wordpress.com/2019/08/main_screen.png)

# Settings

The settings dialog allows you to change the coder name. Multiple coders can code the same text. Checking the Show IDs box displays ID columns for data stored in various tables. The default language of QualCoder is English. Currently French and German are alternative options. These alternatives have not been thoroughly reviewed for accuracy of translations.
Project backup options are set here too. When the backup every time project is opened is checked, an additional option is to choose to backup the audio/video files. For completeness of backups it is recommended to back up audio and video, however this may slow down opening of the software if you have many large files.

![settings](https://qualcoder.files.wordpress.com/2019/08/settings.png)

# Files and Cases Menu
##  Manage Files
You will usually want to load text files into QualCoder prior to coding. You can import text from plain text documents, docx, odt, epub and pdf documents. Pdf importing can sometimes be problematic. Another option is to manually enter text from within QualCoder. You can also load image files in the following formats: jpg, jpeg, png and gif. 

Video (mov, mp4, wmv format) and audio files (wav, mp3 format) can be imported. Loading an audio or video file will also automatically create a blank text transcribed file. This file will have the same name as the audio or video file, but have a '.transcribed' suffix. Initially, this text transcription will be empty. You can transcribe the file your self or get the file professionally transcribed and copy and paste the text into this file.

Filenames should only contain typical filename characters, e.g. a-z 0-9 _ - space (). Otherwise, when exporting a text file, unusual characters in the file name will cause an error. Exporting is only available for text files, if you need to copy an image or other media, open the relevant folder inside the .qda folder to copy the media.

Attributes are variables that can be used to describe or classify the files. These can be added here or through the Manage Attributes menu option.

![manage files dialog](https://qualcoder.files.wordpress.com/2019/01/manage_files.png)

As a practical example: Open the Manage Files dialog. In the Examples folder import the following files: ID1.docx, ID2.odt, transcript.txt and the miguel-henriques.jpg.

You can open an audio or video file to view. This opens two windows, one for viewing the video and one for the controls and a transcript, shown below. The transcript text file must have the same name as the video file, but have a '.transcribed' suffix. The transcribed text file is stored within the sqlite database, but can be exported to a text file. 

If you have a .srt file (a translation file that is read by VLC) you can place this alongside the video inside the project folder, in the video folder, shown in the image below. When the video is played, the translation wording will be shown as subtitles in the video. Also, if you open the .srt file in a text editor, copy and paste this into the video.mp4.transcribed text file. Then this text will be shown as the transcription for the video. 

Transcriptions should ideally contain timestamps indicating when the text is being pronounced during the video. The following formats are recognised by QualCoder, where SSS are milliseconds:

[hh:mm:ss] [mm:ss] [hh.mm.ss] [mm.ss] 

#hh:mm:ss.SSS# 

hh:mm:ss,SSS --> hh:mm:ss,SSS

The video file might contain multiple audio tracks. There is a drop down box that allows you to choose another audio track.


# Manage cases

Open the Manage Cases dialog, shown here:

![Manage cases dialog](https://qualcoder.files.wordpress.com/2019/01/cases.png?w=990)

Cases are useful for seeing text and imaged linked to particular cases and for assigning attributes such as age and gender to interview participants. You can add a memo of notes to each case and rename a case by double-clicking on a case name.

Practical example: Add the three students (or cases) here by clicking the Add case button. Call each student: ID1, ID2 and ID3.

Now, add each student’s file to each student. Click on a case, say ID1, then click the Add file to case button. Select the ID1.docx file. Add the ID2.odt file to ID2 and add the miguel-henriques.jpg to ID3.

Use the Open file to view and assign text to case button and open file ID1.docx and select case ID1. You will see the text will be underlined in red which indicates this text is associated with this case.

Now open the transcript.txt file. Notice the transcript begins with a student id inside square brackets [ ].

![Transcript](https://qualcoder.files.wordpress.com/2019/01/cases_trans_1.png)

Try automatically assigning text to ID1 by selecting case ID1 then clicking the Auto assign file text button. You will be asked which file or files to assign the case to. Select transcript.txt from the list. Next you need to enter the start and end marks. The start mark will be ‘[id1]’ and the end mark will be ‘[‘, note this is case sensitive so that is why you use the lower case here.

![Auto-assign start and end marks](https://qualcoder.files.wordpress.com/2019/01/automarking_case.png?w=443&h=232)

Now select the case ID1 and see the assigned text.

![Transcript portions assigned to a case](https://qualcoder.files.wordpress.com/2019/01/autocase_highlighted.png)

You can also select a case, manually highlight text, and right-click to mark – or assign -the text to the selected case.

Importing attributes for the cases. You can import attributes from a CSV file. The first row must contain the attribute headings. The first column must contain matching case names (for this example: ID1, ID2, ID3). Note that this is case sensitive. Open the attributes.csv file in the Examples folder to see how it is laid out.

For this example – delete all the cases shown. Then, import the attributes from the attributes.csv file through the Import Attributes dialog. You will again need to link the files and file text to each case.

## Import survey

This asks for a CSV file to be imported. You can try importing the survey.csv file in the Examples folder. 

Survey files must be in a CSV format, that is comma delimited format, or another delimiter (tabs are commonly used too). For tab-delimited files type ta, tb, or tab in the Delimiter box so that QualCoder knows the csv file is tab delimited. The first row must contain the headings for attributes. The first column must contain the unique identifiers for each survey respondent. QualCoder will determine if the other columns (attributes) are Numeric or Character. QualCoder cannot determine if an attribute is qualitative data. You must right-click and change the field type from character to qualitative for those fields that need to be qualitative. 

![Import survey dialog](https://qualcoder.files.wordpress.com/2019/01/change_to_qual.png)

When you click on the OK button, the cases and their attributes will be added. The qualitative column will be converted to a file which will be named with the column name plus the current date and time. Each respondent's row will be prepended with [the unique id] so that you can identify each respondent. Also, the text for each respondent will be automatically linked to the corresponding case.

## Attributes menu

Attributes are variables associated with files or cases. They can be useful to add context to the text analysis. Open the Manage Attributes dialog. You can add, delete, rename and add memo notes to attributes.

It is not the intention for QualCoder to perform statistical analyses of the attributes. It would be preferable to use dedicated statistical software such as R (https://www.r-project.org/) or other such software.

![Attributes dialog](https://qualcoder.files.wordpress.com/2019/01/manage_attributes.png)

##  Coding text

Select Code text from the Coding menu. This is the central dialog for assigning codes to text. Once text segments are coded, hovering the mouse over the coding shows the code name as a tooltip. Clicking on the coded segment also shows the code name. Press the View File button to select a file to open for coding. Create a new code by right-clicking in the left hand window. Codes can also be assigned a colour by right-clicking on the code and selecting the change code colour option. Other options from the right-click menu include adding a memo to the code, deleting the code, renaming, adding a new code, and adding a new category.

Select a code, then select some text. Right-click and mark the text to assign it to the selected code. Hover the mouse pointer over coded text to see a tooltip of the code. Coded text can be uncoded by clicking on the text segment and pressing the Unmark button.

![Coding text](https://qualcoder.files.wordpress.com/2019/01/coding1.png?w=990)

Add an annotation (like a memo for a text segment) to a text selection. The text will become **bold** to mark the position of the annotation.

![annotation](https://qualcoder.files.wordpress.com/2019/01/annotation.png?w=429&h=240)

You can also automatically code text segments using the Auto Code button. Enter the text you want to autocode. A dialog asks for one or more files to autocode. All matching text will be assigned the selected code.

##  Categories and codes

Categories are used to organise codes. Categories are organised hierarchically in a tree structure. The cat symbol denotes a category, whereas the writing-paper symbol denotes a code.

You can move codes into categories and move categories into larger categories. You can move categories and codes out of their current position. Codes and categories can be merged by dropping a code onto a code or a category onto a category.

![categories and codes](https://qualcoder.files.wordpress.com/2019/01/category_with_codes.png)

##  Coding images

Images can be coded in a similar way to text coding. Select a code. Left-click and drag to highlight the area you want to assign to the code. Right-click will open a menu where you can remove the coding or add a memo. At the bottom of the screen there is a slider control to re-size the image.

![coding image](https://qualcoder.files.wordpress.com/2019/01/image_coding.png?w=618&h=445)

## Coding audio and video

When coding audio or video, two windows are displayed, shown below. One window has the audio or video playing. The other window has the controls and a button to begin and end a coded segment. The controls window shows the codes in the bottom left pane and the .transcribed file text is shown in the bottom right pane. The transcription text can also be coded and annotated in this window. Right-clicking on a timestamp will give you a menu option to go to that section of the video. If a video has multiple audio tracks, you can cane the audio track too. Checking the scroll checkbox allows the transcript to scroll in time with the video, based on detected timestamps, however, you need to uncheck the scroll to be able to code the transcript.

Once a segment is made using the _Start segment/Stop segment_ button this can be assigned to a code by right clicking on the relevant code and assigning the segment. 

![coding a/v](https://qualcoder.files.wordpress.com/2019/08/video-coding.png)

Coding stripes for the coded segments are shown in the upper pane. Hovering the mouse over each stripe shows the code name, time segment and any memo attached to that coded segment. Right clicking on a coded segment stripe shows a menu that can be used to edit he memo or delete the coded segment. Coded stripes are shown on various lines so that they do not overlap. 

The transcript text can also be coded and annotated in this dialog. However, when the Scroll transcript check box is checked, this cannot be performed. Playing the video when this is check will scroll the transcript using the timestamps in time with the video.

##  Codebook

A codebook is a list of your codes. Each code memo should detail the reasons for the purpose of each code. The codebook can be exported to a text file. The codebook also shows the frequency of the codes used (from all coders). Example codebook output is shown below. As codes and categories are put in a tree like structure the double minus ‘–‘ indicates the subordinate codes and categories within a category.

##  Node graph

A graph of categories and codes is displayed. There are several options to change what is shown – such as Black and White, All or selected categories.

Each code or category can be moved around by clicking near the edge of the box and dragging it around. Clicking on the text allows you to temporarily change the code or category wording. Right-clicking in a code gives a menu of options such as displaying the memo, or displaying all the case or file text that has been coded with the selected code.

![Node graph](https://qualcoder.files.wordpress.com/2019/01/node-graph.png)







