#  Manage Files
Load text files into QualCoder prior to coding. You can import text from plain text documents, docx, epub, md, odt and pdf documents. 
Pdf importing is problematic and may need editing as formatting is lost. Large Pdf files take a long time to import. QualCoder extracts text from the Pdf files using pdfminer.six, but you may choose to use another extraction program for the plain text, suggestions include: www.pdf2go.com/  www.pdfmate.com/pdf-converter-free.html  https://pandoc.org/ and then copy the plain text across.

The following image files formats can be loaded: jpg, jpeg and png. 

You can create and enter text into a file stored in the database, by pressing the Create pencil icon. 

If you import really large text files, when coding QualCoder can split the files into 50,000 character chunks to reduce the slowness of the program. The best option when importing large text files is to split them into separate sections and load those smaller sections as separate files instead. Give each filename some ordered logic too, e.g. book_chap01.txt, book_chap02.txt.

There are a few sample files in the Examples folder. These can be used to test importing files of different document formats and of importing an image. There are also example files to test importing case attributes, and for importing a survey.

Video (mov, mp4, wmv format) and audio files (wav, mp3 format) can be imported. Loading an audio or video file will also automatically create a blank text transcribed file. This file will have the same name as the audio or video file, but have a '.transcribed' suffix. Initially, this text transcription will be empty. You can transcribe the file yourself or get the file professionally transcribed and copy and paste the text into this file.

A right-click context menu allows you to view, export, delete a current file. The menu also allow you to re-order the files according to alphabet, date, and file-type and when right clicking in the name or date columns. You can show only selected attribute types, if the right-click occurs in an attribute column.

Filenames can be changed in the database. The original file names of the actual files will not be changed.

The red X button is an option to select multiple files for deletion.
 The question mark '?' opens this help page.

Files can be linked to rather than imported into the QualCoder project folder. The diagonal link icon performs this task. The two other icons with links allow you to import a linked files into the project folder, and to remove a file from the project folder but keep a link to the file.

Attributes are variables that can be used to describe or classify the files. These can be added here (using the blue + button) or through the Manage Attributes menu option.

Each file is preceded with an icon that describes the type of file. An icon with a black T and red play button indicates text transcription stored in the database that is associated with and audio or video file. Other columns show the file name, date of creation/upload, association with cases and other attributes. 

![Manage Files tab](https://qualcoder.files.wordpress.com/2021/10/manage_files.png?)


Files can be viewed either by right-click menu on the file, or by clicking the eye icon. This is where transcripts for audio and video can be entered, when viewing an audio or video file.

As a practical example: Open the Manage Files dialog. In the Examples folder import the following files: ID1.docx, ID2.odt, transcript.txt and the miguel-henriques.jpg.

## Text file creation and editing

Manage Files > Create text file or View text file. Manage files View Audio/Video (with the transcribed text file shown).

Text files can be edited providing no coding or annotations or case assignment have been performed with the text file. Copying and pasting text from elsewhere (e.g. web page) may show formatting from the copy/paste (e.g. bold, italic, foreground and background colours) until the text file is re-opened.

Sections of the text file or audio/video transcribed file will have sections of text underlined in green (case assigned), yellow (annotation) or red (coded). Text can be edited even after the text is coded or annotated or assigned (fully or partially) to a case. 

You can select text that is not underlined and copy/replace without problems. You can click on a position (**without selecting a section of text**) to then type, delete, or paste text. This can occur in underlined (coded, annotated, case-assigned) or not underlined (not coded/annotated/case-assigned) text locations. You will see the underlines shift as text is added or removed.

**There are some limitations: It is best to avoid selecting sections of text to delete (or to type or paste over) if those sections have a combination of not underlined (not coded/annotated/case-assigned) and underlined (coded, annotated, case-assigned). The reason is that positions of the underlying codes/annotations/case-assigned may not correctly match as intended. If you have made a change that you think has affected these coded/annotated/case-assigned positions badly, exit the text editing window by pressing the Cancel button.**


## Audio and Video files

You can open an audio or video file to view. for video, this opens two windows, one for viewing the video and one for the controls and a transcript, shown below. The transcript text file must have the same name as the video file, but have a '.transcribed' suffix, e.g. video.mp4.transcribed (versions 2.7 and below). Version 2.8 and above, the transcription file name defaults to video.mp4.txt.

**Important: When an audio or video file is loaded into QualCoder a blank text transcription file is automatically created. Version 2.7 and below it is named in this format: videoname.mp4.transcribed. Versions 2.8 and above are named in this format: videoname.mp4.txt.**

The transcribed text file is created and stored within the database, and can be exported to a text file. The file can be edited.  **Important note: The edits occur within the database. An original text file is NOT changed. Transcriptions cannot be linked as an external file. Transcription files can be exported as text files.** 


If you have a .srt file (a translation file that is read by VLC) you can place this alongside the video inside the project folder, in the video folder, shown in the image below. When the video is played, the translation wording will be shown as subtitles in the video. Also, if you open the .srt file in a text editor, copy and paste this into the video.mp4.transcribed text file. Then this text will be shown as the transcription for the video. 

![Audio Video viewing dialog](https://qualcoder.files.wordpress.com/2020/12/viewav3.png)

If you have ffmpeg installed a waveform and spectrogram are shown. This work on Ubuntu - but have not tested this on Windows. To change the display from a waveform to a spectrogram and back use Ctrl I and Ctrl U. If the audio files has multiple audio tracks, only the first track is shown for the waveform or spectrogram.

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

### Speech to text

QualCoder has a speech to text function. The [ffmpeg](https://www.ffmpeg.org/) software must be installed for this to work. When an audio or video file is added to the QualCoder project an empty transcription file is created. The cogs button activates this function, but only if there is no text entered into the transcription file. First, open (view) the audio/video from Manage Files.

Speech to text allows use of several online third-party services. Most require sign up. Google does not but is limited to 50 requests of the service per day (e.g. 50 x 1 minute audio segments). QualCoder converts the audio file into 30 or 60 second chunks and adds a timestamp for each of these. Each chunk is provided to the online service which then takes a few second to convert to text.

Language options are entered into the Language box, or might be configured when you signed up to a service such as Houndify or Wit.ai. Language options are entered as text in format like: en-US, fr-FR, de-DE, es-ES, pt-PT, pt-BR.

### Transcriptions that have codes, annotations and / or case-assigned

Sections of the text file or audio/video transcribed file will have sections of text underlined in green (case assigned), yellow (annotation) or red (coded). Text can be edited even after the text is coded or annotated or assigned (fully or partially) to a case. 

You can select text that is not underlined and copy/replace without problems. You can click on a position (**without selecting text**) to then type, delete, or paste text. This can occur in underlined (coded, annotated, case-assigned) or not underlined (not coded/annotated/case-assigned) text locations. You will see the underlines shift as text is added or removed.

**There are some limitations: It is best to avoid selecting sections of text to delete (or to type or paste over) if those sections have a combination of not underlined (not coded/annotated/case-assigned) and underlined (coded, annotated, case-assigned). The reason is that positions of the underlying codes/annotations/case-assigned may not correctly match as intended. If you have made a change that you think has affected these coded/annotated/case-assigned positions badly, exit the text editing window by pressing the Cancel button.**


