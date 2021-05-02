#  Manage Files
Load text files into QualCoder prior to coding. You can import text from plain text documents, docx, epub, md, odt and pdf documents. 
Pdf importing is problematic and may need editing as formatting is lost. Large Pdf files take a long time to import. QualCoder extracts text from the Pdf files using pdfminer.six, but you may choose to use another extraction program for the plain text, suggestions include: www.pdf2go.com/  www.pdfmate.com/pdf-converter-free.html  https://pandoc.org/ and then copy the plain text across.

You can image files in the following formats: jpg, jpeg and png. You can also create and enter text into a file stored in the database, by pressing the Create pencil icon. 

There are a few sample files in the Examples folder. These can be used to test importing files of different document formats and of importing an image. There are also example files to test importing case attributes, and for importing a survey.

Video (mov, mp4, wmv format) and audio files (wav, mp3 format) can be imported. Loading an audio or video file will also automatically create a blank text transcribed file. This file will have the same name as the audio or video file, but have a '.transcribed' suffix. Initially, this text transcription will be empty. You can transcribe the file yourself or get the file professionally transcribed and copy and paste the text into this file.

A right-click context menu allows you to view, export, delete a current file. The menu also allow you to re-order the files according to alphabet, date, and file-type and when right clicking in the name or date columns. You can show only selected attribute types, if the right-click occurs in an attribute column.

The red X button is an option to select multiple files for deletion.
 The question mark '?' opens this help page.

Files can be linked to rather than imported into the QualCoder project folder. The diagonal link icon performs this task. The two other icons with links allow you to import a linked files into the project folder, and to remove a file from the project folder but keep a link to the file.

Attributes are variables that can be used to describe or classify the files. These can be added here (using the blue + button) or through the Manage Attributes menu option.

![Manage Files tab](https://qualcoder.files.wordpress.com/2021/05/files.png?resize=550%2C500)


Files can be viewed either by right-click menu on the file, or by clicking the eye icon. This is where transcripts for audio and video can be entered, when viewing an audio or video file.

As a practical example: Open the Manage Files dialog. In the Examples folder import the following files: ID1.docx, ID2.odt, transcript.txt and the miguel-henriques.jpg.

## Text files creation and editing

Text files can be edited providing no coding or annotations or case assignment have been performed with the text file. Copying and pasting text from elsewhere (e.g. web page) may show formatting from the copy/paste (e.g. bold, italic, foreground and background colours) until the text file is re-opened.

If the file has already had some coding or annotations assigned, the sections of the text file will be shown underlined in red. Editing text is now restricted to small text selections up to 20 characters. This is achieved by selecting some text then right click and select the edit text option.

## Audio and Video files

You can open an audio or video file to view. for video, this opens two windows, one for viewing the video and one for the controls and a transcript, shown below. The transcript text file must have the same name as the video file, but have a '.transcribed' suffix. The transcribed text file is stored within the sqlite database, but can be exported to a text file. 

If you have a .srt file (a translation file that is read by VLC) you can place this alongside the video inside the project folder, in the video folder, shown in the image below. When the video is played, the translation wording will be shown as subtitles in the video. Also, if you open the .srt file in a text editor, copy and paste this into the video.mp4.transcribed text file. Then this text will be shown as the transcription for the video. 

![Audio Video viewing dialog](https://qualcoder.files.wordpress.com/2020/12/viewav3.png)

## Transcribing audio and video

To transcribe open the Mange files menu option, then view the audio or video file. The audio/video will load and there will be a text area to enter transcribed text. QualCoder does not have an automated audio to text feature. Other services such as otter.ai may assist you.
Transcriptions should ideally contain timestamps indicating when the text is being pronounced during the video. The following formats are recognised by QualCoder, where SSS are milliseconds:

[hh:mm:ss] 

[mm:ss] 

[hh.mm.ss] 

[mm.ss] 

For the above, brackets can be []  or {}. These can be changed in the Settings menu.

#hh:mm:ss.SSS# 

hh:mm:ss,SSS --> hh:mm:ss,SSS

The video file might contain multiple audio tracks. There is a drop down box that allows you to choose another audio track.

Transcriptions may contain speaker names indicating who is speaking. Speaker names are bracketed in this format: [name] or {name}. Dots ‘.’ and colons ‘:’ cannot be used in speaker names.

Manually transcribing audio and video is helped with some keyboard shortcuts. Transcribing and adding or editing text can only occur if the existing text has no codes or annotations. Copying and pasting text from elsewhere (e.g. web page) may show formatting from the copy/paste (e.g. bold, italic, foreground and background colours) until the text file is re-opened.

Transcribing and adding or editing text can only occur if the existing text has no codes or annotations.

The shortcuts available are:

Ctrl R		Rewind 5 seconds

Alt R		Rewind 30 seconds

Alt F		Forward 30 seconds

Ctrl S or Ctrl P	Stop/Start toggle audio/video. From stop to play will rewind 2 seconds.

Ctrl Shift > Increase play rate up to 2 times

Ctrl Shift < Decrease play rate down to 0.1 

The above controls are also available from the toolbar icons.

Ctrl T		Insert timestamp in this format: [hh.mm.ss]

Ctrl +N		Add a speaker name. This also pauses the audio/video.

Ctrl D		Delete one or more speaker names.

Ctrl 1 to 8	Insert speaker name in this format: [name]


