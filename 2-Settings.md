
# Settings

The settings dialog allows you to change several features including language, coder name and font type and font size. Multiple coders can code the same text. A new coder name can be entered in the text box. You can choose an existing coder from the drop down box.

The default language of QualCoder is English. Currently French, German, Greek, Italian, Japanese and Spanish are alternative languages. These languages have not been thoroughly reviewed for accuracy of translations (especially Greek, Japanese, Spanish). When changing a language, you need to close then reopen QualCoder for the change to occur.

Checking the Show IDs box displays the numeric IDs for codes files cases and more. These IDs may be useful when writing sql queries.

Checking the Dark mode box, changes the overall look of QualCoder from dark text on a light background, to light text on a dark background.

For transcribing audio and video, the time format and bracket type can be selected.

Project backup can be set to automatically backup every hour, or no backup. QualCoder keeping the most recent five backups with a date and hour time stamp. The backup name is: _projectname_BKP_yyyymmdd_hh.qda_  Where _hh_ is 24 hour time. This also means multiple backups are not done within an hour. So a new backup cannot overwrite another backup created within the same hour. Up to five backups are kept, **older backups are deleted**. 

Rename or move to another location particular backups that you need to keep. When the backups are set, an additional option is to choose to backup the audio/video files. For completeness of backups it is recommended to back up audio and video, however this may slow down opening of the software if you have many large files. Alternatively you can link to large audio/video files rather than import them into the project folder.

The default project directory is where many file operations will default to, for export or looking to import files.

![settings](https://qualcoder.files.wordpress.com/2020/08/settings.png)



#  Create a new project

Create a new project under the ‘Project’ menu, call it test. The project will be saved as test.qda. Test.qda is actually a folder containing subfolders which hold the database and other files. Additionally, in your home folder QualCoder will create a .qualcoder folder with a QualCoder.log file for logging events and a config.ini file which will contain a lot of settings such as the current coder’s name, preferred fonts, language and a preferred working directory.

Under the Project menu click on Project memo. This is where you can put notes about your overall project.

The Action Log tab displays various changes that are made when using QualCoder. The main window has a menu bar at the top full of options. There are four tabs for: _action log_, _manage_, _reports_ and _coding_ (text coding shown below).

![main screen](https://qualcoder.files.wordpress.com/2021/02/tabbed.png)










