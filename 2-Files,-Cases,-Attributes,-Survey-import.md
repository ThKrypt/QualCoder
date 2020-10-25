
There are a few sample files in the Examples folder. These can be used to test importing files of different document formats and of importing an image. There are also example files to test importing case attributes, and for importing a survey.

#  Create a new project

Create a new project under the ‘Project’ menu, call it test. The project wil be saved as test.qda. Test.qda is actually a folder containing subfolders which hold the database and other files. Additionally, in your home folder QualCoder will create a .qualcoder folder with a QualCoder.log file for logging events, including hopefully all software errors and exceptions and a QualCoder_settings.txt file which will contain the current coder’s name, preferred fonts and a preferred working directory.

Under the Project menu click on Project memo. This is a memo about your project. Type “A test QDA project” and click the OK button.

The main window displays various changes that are made when using QualCoder. You will notice the main window displays the following, with a menu bar at the top:

![main screen](https://qualcoder.files.wordpress.com/2019/08/main_screen.png)

# Settings

The settings dialog allows you to change the coder name. Multiple coders can code the same text. Checking the Show IDs box displays ID columns for data stored in various tables. The default language of QualCoder is English. Currently French, German, Japanese, Spanish are alternative options. These alternatives have not been thoroughly reviewed for accuracy of translations.
Project backup options are set here too. When the backups are set, an additional option is to choose to backup the audio/video files. For completeness of backups it is recommended to back up audio and video, however this may slow down opening of the software if you have many large files.
Backups occur every hours, with QualCoder keeping the most recent five backups. Rename or move to another location particular backups that you need to keep.

![settings](https://qualcoder.files.wordpress.com/2019/08/settings.png)

# Files and Cases Menu
##  Manage Files
You will usually want to load text files into QualCoder prior to coding. You can import text from plain text documents, docx, odt, epub and pdf documents. Pdf importing can sometimes be problematic. Another option is to manually enter text from within QualCoder. You can also load image files in the following formats: jpg, jpeg and png. 

Video (mov, mp4, wmv format) and audio files (wav, mp3 format) can be imported. Loading an audio or video file will also automatically create a blank text transcribed file. This file will have the same name as the audio or video file, but have a '.transcribed' suffix. Initially, this text transcription will be empty. You can transcribe the file your self or get the file professionally transcribed and copy and paste the text into this file.

Filenames should only contain typical filename characters, e.g. a-z 0-9 _ - space (). Otherwise, when exporting a text file, unusual characters in the file name will cause an error. Exporting is only available for text files, if you need to copy an image or other media, open the relevant folder inside the .qda folder to copy the media.

Attributes are variables that can be used to describe or classify the files. These can be added here or through the Manage Attributes menu option.

![manage files dialog](https://qualcoder.files.wordpress.com/2019/01/manage_files.png)

As a practical example: Open the Manage Files dialog. In the Examples folder import the following files: ID1.docx, ID2.odt, transcript.txt and the miguel-henriques.jpg.

### Text files

Text files can be easily edited if they have no codes, annotations or cases assigned to them. Once these has been assigned, editing is limited to short text segments up to 20 characters long. To edit, select the text and right click to get a menu option to edit the text segment.

### Audio and Video files

You can open an audio or video file to view. This opens two windows, one for viewing the video and one for the controls and a transcript, shown below. The transcript text file must have the same name as the video file, but have a '.transcribed' suffix. The transcribed text file is stored within the sqlite database, but can be exported to a text file. 

If you have a .srt file (a translation file that is read by VLC) you can place this alongside the video inside the project folder, in the video folder, shown in the image below. When the video is played, the translation wording will be shown as subtitles in the video. Also, if you open the .srt file in a text editor, copy and paste this into the video.mp4.transcribed text file. Then this text will be shown as the transcription for the video. 

Transcriptions should ideally contain timestamps indicating when the text is being pronounced during the video. The following formats are recognised by QualCoder, where SSS are milliseconds:

[hh:mm:ss] 

[mm:ss] 

[hh.mm.ss] 

[mm.ss] 

For the above, brackets can be []  or {}. These can be changed in the Settings menu.

#hh:mm:ss.SSS# 

hh:mm:ss,SSS --> hh:mm:ss,SSS

The video file might contain multiple audio tracks. There is a drop down box that allows you to choose another audio track.

### Transcribing audio and video

Speaker names are bracketed in this format: [name] or {name}. Dots ‘.’ and colons ‘:’ cannot be used in speaker names.
Manually transcribing audio and video is helped with some keyboard shortcuts. Transcribing and adding or editing text can only occur if the existing text has no codes or annotations.

The shortcuts available are:

ctrl R		Rewind 5 seconds

Alt R		Rewind 30 seconds

Alt F		Forward 30 seconds

Ctrl S or Ctrl P	Stop/Start toggle audio/video. From stop to play will rewind 2 seconds.

Ctrl T		Insert timestamp in this format: [hh.mm.ss]

Ctrl +N		Add a speaker name. This also pauses the audio/video.

Ctrl D		Delete one or more speaker names.

Ctrl 1 to 8	Insert speaker name in this format: [name]

Ctrl Shift > Increase play rate up to 2 times

Ctrl Shift < Decrease play rate down to 0.1 


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








