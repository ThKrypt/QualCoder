There are a few sample files in the Examples folder. These can be used to test importing files of different document formats and of importing an image. There are also example files to test importing case attributes, and for importing a survey.

#  Create a new project

Create a new project under the ‘Project’ menu, call it test. The project wil be saved as test.qda. Test.qda is actually a folder containing subfolders which hold the database and other files. Additionally, in your home folder QualCoder will create a .qualcoder folder with a QualCoder.log file for logging events, including hopefully all software errors and exceptions and a QualCoder_settings.txt file which will contain the current coder’s name, preferred fonts and a preferred working directory.

Under the Project menu click on Project memo. This is a memo about your project. Type “A test QDA project” and click the OK button.

The main window displays various changes that are made when using QualCoder. You will notice the main window displays the following, with a menu bar at the top:

IMAGE

# Settings

The settings dialog allows you to change the coder name. Multiple coders can code the same text. Checking the Show IDs box displays ID columns for data stored in various tables.The default language of QualCoder is English. Currently French and German are alternative options.

IMAGE

# Files and Cases Menu
##  Manage Files
You will usually want to load text files into QualCoder prior to coding. You can import text from plain text documents, docx, odt, epub and pdf documents. Pdf importing can sometimes be problematic. Another option is to manually enter text from within QualCoder. You can also load image files in the following formats: jpg, jpeg, png and gif. 

Video (mov, mp4, wmv format) and audio files (wav, mp3 format) can be imported. Loading an audio or video file will also automatically create a blank text transcript file. This file will have the same name as the audio or video file, but have a '.transcribed' suffix. Initially, this text transcription will be empty. You can transcribe the file your self or get the file professionally transcribed and copy and paste the text into this file.

Filenames should only contain typical filename characters, e.g. a-z 0-9 _ - space (). Otherwise, when exporting a text file, unusual characters in the file name will cause an error. Exporting is only available for text files, if you need to copy an image or other media, open the relevant folder inside the .qda folder to copy the media.

Attributes are variables that can be used to describe or classify the files. These can be added here or through the Manage Attributes menu option.

IMAGE

As a practical example: Open the Manage Files dialog. In the Examples folder import the following files: ID1.docx, ID2.odt, transcript.txt and the miguel-henriques.jpg.

You can open an audio or video file to view. This opens two windows, one for viewing the video and one for the controls and a transcript, shown below. The transcript text file must have the same name as the video file, but have a '.transcribed' suffix.

IMAGE

# Manage cases

Open the Manage Cases dialog, shown here:

IMAGE

Cases are useful for seeing text and imaged linked to particular cases and for assigning attributes such as age and gender to interview participants. You can add a memo of notes to each case and rename a case by double-clicking on a case name.

Practical example: Add the three students (or cases) here by clicking the Add case button. Call each student: ID1, ID2 and ID3.

Now, add each student’s file to each student. Click on a case, say ID1, then click the Add file to case button. Select the ID1.docx file. Add the ID2.odt file to ID2 and add the miguel-henriques.jpg to ID3.

Use the Open file to view and assign text to case button and open file ID1.docx and select case ID1. You will see the text will be underlined in red which indicates this text is associated with this case.

Now open the transcript.txt file. Notice the transcript begins with a student id inside square brackets [ ].

IMAGE

Try automatically assigning text to ID1 by selecting case ID1 then clicking the Auto assign file text button. You will be asked which file or files to assign the case to. Select transcript.txt from the list. Next you need to enter the start and end marks. The start mark will be ‘[id1]’ and the end mark will be ‘[‘, note this is case sensitive so that is why you use the lower case here.

IMAGE

Now select the case ID1 and see the assigned text.clicking in a code gives a menu of options such as displaying the memo, or displaying all the case or file text that has been coded with the selected code.

IMAGE









