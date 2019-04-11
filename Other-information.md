The qda data folder contains folders for imported documents, images and audio and video. It also contains the sqlite database, named data.qda, to store coding data.

QualCoder creates QualCoder.log and QualCoder_settings.txt files in a .qualcoder folder in your home directory. The settings file contains the name of the current coder, a default working directory and choice of font. The log file records program errors and some user actions.

QualCoder is written in python 3 using Qt for the graphical interface. A Sqlite database is used to store the coding data.

# Future plans

Currently QualCoder has only used on Ubuntu, Linux Mint, Lubuntu and Windows 10, with some testing on MacOS. Further testing on different operating systems is required.

In Windows, reports exported in ODT format are okay, but some images may overlap when the ODT file opened with Microsoft Word rather than opened with LibreOffice.


Some potential plans for the future are to add functionality.
Coding: 
    • Possibly add alternative ways to view text coding.
Reports: 
    • Some statistics: word count, possibly add bar or pie charts for some attributes.
    • Possibly look at text mining functionality
    • Possibly have an html report with embedded audio/video.
General:
* Multi-language support
