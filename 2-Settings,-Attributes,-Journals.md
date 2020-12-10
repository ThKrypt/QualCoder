
# Settings

The settings dialog allows you to change several features including language, coder name and font type and font size. Multiple coders can code the same text. A new coder name can be entered in the text box. You can choose an existing coder from the drop down box.

The default language of QualCoder is English. Currently French, German, Greek, Italian, Japanese and Spanish are alternative languages. These languages have not been thoroughly reviewed for accuracy of translations (especially Greek, Japanese, Spanish). When changing a language, you need to close then reopen QualCoder for the change to occur.

Checking the Show IDs box displays the numeric IDs for codes files cases and more. These IDs may be useful when writing sql queries.

For transcribing audio and video, the time format and bracket type can be selected.

Project backup can be set to automatically backup every hour, or no backup. QualCoder keeping the most recent five backups with a date and hour time stamp. The backup name is: _projectname_BKP_yyyymmdd_hh.qda_  Where _hh_ is 24 hour time. This also means multiple backups are not done within an hour. So a new backup cannot overwrite another backup created within the same hour. Up to five backups are kept, older ones are deleted. 

Rename or move to another location particular backups that you need to keep. When the backups are set, an additional option is to choose to backup the audio/video files. For completeness of backups it is recommended to back up audio and video, however this may slow down opening of the software if you have many large files.

The default project directory is where many file operations will default to, for export or looking to import files.

![settings](https://qualcoder.files.wordpress.com/2020/08/settings.png)



#  Create a new project

Create a new project under the ‘Project’ menu, call it test. The project will be saved as test.qda. Test.qda is actually a folder containing subfolders which hold the database and other files. Additionally, in your home folder QualCoder will create a .qualcoder folder with a QualCoder.log file for logging events and a config.ini file which will contain a lot of settings such as the current coder’s name, preferred fonts, language and a preferred working directory.

Under the Project menu click on Project memo. This is where you can put notes about your overall project.

The main window displays various changes that are made when using QualCoder. You will notice the main window has a menu bar at the top full of options. There is also another tab for typing any temporary notes that you wish to make. These notes are not stored.

![main screen](https://qualcoder.files.wordpress.com/2020/08/mainscreen.png)


# Attributes

Attributes are variables associated with files or cases. They can be useful to add context to the text analysis. Open the Manage Attributes dialog. You can add, delete, rename and add memo notes to attributes.

It is not the intention for QualCoder to perform statistical analyses of the attributes. It would be preferable to use dedicated statistical software such as R (https://www.r-project.org/) or other such software.

![Attributes dialog](https://qualcoder.files.wordpress.com/2019/01/manage_attributes.png)

# Journals
You can record your thoughts when coding your data in journals. Make use of these to develop ideas and themes.










