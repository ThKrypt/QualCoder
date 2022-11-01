# Data structures

The qda data folder contains folders for imported documents, images and audio and video. It also contains the sqlite database, named data.qda, to store coding data.

QualCoder creates QualCoder.log and QualCoder_settings.txt files in a .qualcoder folder in your home directory. The settings file contains the name of the current coder, a default working directory and choice of font. The log file records program errors and some user actions.

QualCoder is written in python 3 using the Qt6 for the graphical interface.


# Future plans

Currently QualCoder is developed on Ubuntu 22.04 and Windows 10/11. Some people have used Qualcoder on Linux Mint, Lubuntu, Fedora, Manjaro/Arch Raspberry Pi, and on MacOS. 

In Windows, reports exported in ODT format are okay, but some images may overlap when the ODT file opened with Microsoft Word rather than opened with LibreOffice Writer.


Some potential plans for the future are to add functionality:


## Reports: 

**Look at alternative ways to visualise codes:**
* Display code frequency in a comparative way - e.g. compare female versus males for the code frequencies using bar charts or other plots

**Look at timeline reporting:**
* Maybe add in a way to display coding from documents in a timeline - drawing from a file data attribute that is created by the end user.

## General:

* Possibly use Qt Multimedia to play A/V rather than rely on the installation of VLC.

* Multi-language support - review of existing translations needed

* Improve REFI-QDA open standard for import and export to other software. Codebook import and export seems OK. Project import and export seems OK but I would still say it is experimental. To review: A/V coded segments, AV sync-points.


#  About the author

Hello, I have many interests including computer programming and research. I completed a PhD in 2014. When doing my PhD I used R as the statistics program of choice. This is where my interest in qualitative data analysis and the use of RQDA came from, which ultimately led to this project.

Originally when doing my PhD I analysed qualitative survey data via a thematic approach using RQDA. I then thought this could be reproduced in Python, so I wrote an earlier version called PyQDA which worked OK at the time.

I thought I would share QualCoder in the hope that it may help others. Software bugs are possible and functionality could be further extended. I also generally work on Linux machines, and sometimes Windows, so this software probably needs further tweaking for best use on Windows. I work on the programming for this in my spare time, it is not my full time job for me.

If and when you use QualCoder and publish your results, I would really appreciate it if you let me know the bibliographic information of your work.
