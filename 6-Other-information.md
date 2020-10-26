
#  Multiple dialog windows

It is possible to have multiple dialog windows open. This is useful if you have run a report, or have a file open for coding, and you want to enter your thoughts into a journal entry. **However there are some limitations**.
 
Some dialog windows are priority windows, so swapping between windows will not be possible, these restricted windows are: Management of files, cases or attributes, survey import and confirmation dialogs (e.g. confirm delete). 

# Data structures

The qda data folder contains folders for imported documents, images and audio and video. It also contains the sqlite database, named data.qda, to store coding data.

QualCoder creates QualCoder.log and QualCoder_settings.txt files in a .qualcoder folder in your home directory. The settings file contains the name of the current coder, a default working directory and choice of font. The log file records program errors and some user actions.

QualCoder is written in python 3 using Qt for the graphical interface. A Sqlite database is used to store the coding data.


# Future plans

Currently QualCoder has only used on Ubuntu, Linux Mint, Lubuntu and Windows 10, with some testing on MacOS. Further testing is required.

In Windows, reports exported in ODT format are okay, but some images may overlap when the ODT file opened with Microsoft Word rather than opened with LibreOffice.


Some potential plans for the future are to add functionality:


Reports: 

    • Some statistics: word count, possibly add bar or pie charts for some attributes.

   • The RQDA Relation functionand Profile Matrix function.

    • Text mining functionality - maybe.

    • Some statistics: word count, possibly add bar or pie charts for some attributes - maybe.

    • Word clouds, word visualisations - maybe.

    • Look at alternative ways to visualise codes

General:

* Multi-language support - some work done on French, German, Japanese, Spanish.

* Improve REFI-QDA open standard for import and export to other software. Codebook import and export seems OK. Project import and export is experimental.

#  About the author

Hello, my name is Colin Curtain and I am a pharmacist and lecturer from Australia. I have many interests including clinical pharmacy, computer programming, research, statistics and clinical decision support. I completed a PhD evaluating computerised clinical decision support in 2014. When doing my PhD I used R as the statistics program of choice. This is where my interest in qualitative data analysis and the use of RQDA came from, which ultimately led to this project.

Originally when doing my PhD I analysed qualitative survey data via a thematic approach using RQDA. I then thought this could be reproduced in Python, so I scripted an earlier version called PyQDA which worked OK at the time.

I thought I would share QualCoder in the hope that it may help others. Software bugs are possible and functionality could be further extended. I also generally work on Linux machines, and sometimes Windows, so this software probably needs further tweaking for best use on Windows. I work on the programming for this in my spare time, it is not my full time job for me.

If and when you use QualCoder and publish your results, I would really appreciate it if you let me know the bibliographic information of your work.
