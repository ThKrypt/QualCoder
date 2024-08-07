
# Settings

The settings dialog allows you to change several features including language, coder name and font type and font size. Multiple coders can code the same text. A new coder name can be entered in the text box. You can choose an existing coder from the drop down box.

The coder name is 'default' when first using QualCoder. When opening another existing project, please make sure the coder name is set to the name you want to use by checking and updating the Settings before you do work on your project.

The default language of QualCoder is English. Currently French, German, Italian, Portuguese and Spanish are alternative languages. These languages have not been thoroughly reviewed for accuracy of translations. When changing a language, you need to close then reopen QualCoder for the change to occur.

Checking the Show IDs box displays the numeric IDs for codes files cases and more. These IDs may be useful when writing sql queries.

There area few options to change the overall look of QualCoder.

For transcribing audio and video, the time format and bracket type can be selected.

Very large text files can slow the coding mode in QualCoder. So a right-click option in Code Text is to load smaller sized chunks of the text. 50,000 characters is the default size, but this can be changed in Settings to smaller sizes for slower computers.

### Backups

Project backup can be set to automatically backup every hour, or no backup. QualCoder keeping the most recent backups with a date and hour time stamp. The backup name is: _projectname_BKP_yyyymmdd_hh.qda_  Where _hh_ is 24 hour time. This also means multiple backups are not done within an hour. So a new backup cannot overwrite another backup created within the same hour. A limited number of backups are kept, **older backups are deleted**. Setting option allows you to choose from 1 to 10 backups.

Rename or move to another location particular backups that you need to keep. When the backups are set, an additional option is to choose to backup the audio/video files. For completeness of backups it is recommended to back up audio and video, however this may slow down opening of the software if you have many large files. Alternatively you can link to large audio/video files rather than import them into the project folder.

The default project directory is where many file operations will default to, for export or looking to import files.


![settings dialog](https://qualcoder.files.wordpress.com/2022/07/settings.png?resize=400%2C400)

#  Create a new project

Create a new project under the ‘Project’ menu, call it test. The project will be saved as test.qda. Test.qda is actually a folder containing subfolders which hold the database and other files. Additionally, in your home folder QualCoder will create a .qualcoder folder with a QualCoder.log file for logging events and a config.ini file which will contain a lot of settings such as the current coder’s name, preferred fonts, language and a preferred working directory. 

If you are using Windows, do not actively use your QualCoder project in the cloud (OneDrive). Instead, use it locally on your computer, but you can store the project folder as a backup in the cloud (OneDrive).

Under the Project menu click on Project memo. This is where you can put notes about your overall project.

The Action Log tab displays various changes that are made when using QualCoder. The main window has a menu bar at the top full of options. There are four tabs for: _action log_, _manage_, _reports_ and _coding_ (coding shown below). Switching directly between tabs is generally OK. But if you are adding/renaming/deleting files in Mange Files or changing codes/code categories in the coding area, it is better to refresh each tab by selecting an option in the Menu. For example, changing files in Manage files , then doing coding or reports - select an option in the Menu for coding or report, rather than clicking directly on the tab for coding or reports.

![Main screen, action log tab](https://qualcoder.files.wordpress.com/2022/07/main_page.png)   














