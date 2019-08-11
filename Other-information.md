# Multiple dialog windows

It is possible to have multiple dialog windows open. This is useful if you have run a report, or have a file open for coding, and you want to enter your thoughts into a journal entry. **However there are some limitations**.

Some dialog windows are priority windows, so swapping between windows will not be possible, these restricted windows are: Management of attributes, survey import and confirmation dialogs (e.g. confirm delete).

The second limitation is that changes in one dialog will not be reflected in the other dialogs. An example here is adding a code in a coding dialog, the added code will not be shown in other coding or reports windows. If you do make changes to highlighting and codes and categories, it is recommended to close and then re-open the other dialog window that you need. This is to ensure that any changes made show up in the other dialog windows. Similarly, highlighting text on the same file in two opened dialog will not be reflected in the other window. A warning, if you have the same journal entry open in two windows, the last window that is closed will be the entry that is saved.

One software/programming quirk is, if you close a dialog (e.g. manage files dialog) and then immediately try to re-open the dialog, it may not open. To get around open and close another dialog, then try opening the manage files dialog.

[Multiple dialog windows](https://qualcoder.files.wordpress.com/2019/08/multiple_dialogs.png?resize=219%2C219)

# Data structures

The qda data folder contains folders for imported documents, images and audio and video. It also contains the sqlite database, named data.qda, to store coding data.

QualCoder creates QualCoder.log and QualCoder_settings.txt files in a .qualcoder folder in your home directory. The settings file contains the name of the current coder, a default working directory and choice of font. The log file records program errors and some user actions.

QualCoder is written in python 3 using Qt for the graphical interface. A Sqlite database is used to store the coding data.

# Future plans

Currently QualCoder has only used on Ubuntu, Linux Mint, Lubuntu and Windows 10, with some testing on MacOS. Further testing on different operating systems is required.

In Windows, reports exported in ODT format are okay, but some images may overlap when the ODT file opened with Microsoft Word rather than opened with LibreOffice.


Some potential plans for the future are to add functionality:

Coding: 

    • Possibly add alternative ways to view text coding.

Reports: 

    • Some statistics: word count, possibly add bar or pie charts for some attributes.

    • Possibly look at text mining functionality

    • Possibly have an html report with embedded audio/video.

    • Some statistics: word count, possibly add bar or pie charts for some attributes.

    • Word clouds, word visualisations

    • Word counts

    • Look at alternative ways to visualise codes

General:

* Multi-language support - some work done on French and German

* Add REFI-QDA open standard for import and export to other software.

#  About the author

Hello, my name is Colin Curtain and I am a pharmacist and lecturer from Australia. I have many interests including clinical pharmacy, computer programming, research, statistics and clinical decision support. I completed a PhD evaluating computerised clinical decision support in 2014. When doing my PhD I used R as the statistics program of choice. This is where my interest in qualitative data analysis and the use of RQDA came from, which ultimately led to this project.

Originally when doing my PhD I analysed qualitative survey data via a thematic approach using RQDA. I then thought this could be reproduced in Python, so I scripted an earlier version called PyQDA which worked OK at the time.

I thought I would share QualCoder in the hope that it may help others. This is still an early version so bugs are possible and functionality could be further extended. I also generally work on Linux machines, and sometimes Windows, so this software probably needs further tweaking for best use on Windows. I work on the programming for this in my spare time, it is not my full time job for me.

If and when you use QualCoder and publish your results, I would really appreciate it if you let me know the bibliographic information of your work.
