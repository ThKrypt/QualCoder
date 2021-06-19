# Data structures

The qda data folder contains folders for imported documents, images and audio and video. It also contains the sqlite database, named data.qda, to store coding data.

QualCoder creates QualCoder.log and QualCoder_settings.txt files in a .qualcoder folder in your home directory. The settings file contains the name of the current coder, a default working directory and choice of font. The log file records program errors and some user actions.

QualCoder is written in python 3(minimum 3.6 version) using Qt5 for the graphical interface.


# Future plans

Currently QualCoder has only used on Ubuntu and Windows 10. With some use on Linux Mint, Lubuntu,Fedora, Raspberry Pi, and on MacOS. Further testing is required.

In Windows, reports exported in ODT format are okay, but some images may overlap when the ODT file opened with Microsoft Word rather than opened with LibreOffice.


Some potential plans for the future are to add functionality:


Reports: 

    • Text mining functionality - maybe.

    • Look at alternative ways to visualise codes

General:

* Multi-language support - some work done but review of existing translations is needed

* Improve REFI-QDA open standard for import and export to other software. Codebook import and export seems OK. Project import and export is experimental. Definitely need to review attribute import/export. A/V coded segments, AV sync-points. Use of Cases / Sets. Memos to text.

# Some videos of QualCoder

https://www.youtube.com/watch?v=9teZO-KVwqk

https://www.youtube.com/watch?v=D2vks2n9d1g&t=928s

https://www.youtube.com/watch?v=cqAy_RJkhvY

#  About the author

Hello, my name is Colin Curtain and I am a pharmacist and lecturer from Australia. I have many interests including clinical pharmacy, computer programming, research, statistics and clinical decision support. I completed a PhD evaluating computerised clinical decision support in 2014. When doing my PhD I used R as the statistics program of choice. This is where my interest in qualitative data analysis and the use of RQDA came from, which ultimately led to this project.

Originally when doing my PhD I analysed qualitative survey data via a thematic approach using RQDA. I then thought this could be reproduced in Python, so I wrote an earlier version called PyQDA which worked OK at the time.

I thought I would share QualCoder in the hope that it may help others. Software bugs are possible and functionality could be further extended. I also generally work on Linux machines, and sometimes Windows, so this software probably needs further tweaking for best use on Windows. I work on the programming for this in my spare time, it is not my full time job for me.

If and when you use QualCoder and publish your results, I would really appreciate it if you let me know the bibliographic information of your work.
