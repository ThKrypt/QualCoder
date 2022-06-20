Welcome to the QualCoder wiki!

The wiki covers instructions to install and use the QualCoder qualitative data analysis software. THe information here refers to the most recent version of QualCoder.

## What is QualCoder?
QualCoder is free, open source software for qualitative data analysis. 
With QualCoder you can code text, images, audio and video, write journal notes and memos. You can categorise codes into a tree-like hierarchical categorisation scheme. Coding for audio and video requires the VLC media player.
Coder comparison reports can be generated for text coding using the Cohen’s Kappa statistic. A graph displaying codes and categories can be generated to visualise the coding hierarchy. Most reports can be exported as html, open document text (ODT) or as plain text files.

QualCoder is designed to be used as client-based software to be used by one person at a time. (A second coder can use the same project on the same computer, or the project folder can be transferred to the second coder's computer). QualCoder is not designed to be multi-accessed at the same time.

QualCoder is written in python 3 (version 3.6 and up) using Qt6 for the graphical interface. A Sqlite database is used to store the coding data. There is also a wordpress site for QualCoder at https://qualcoder.wordpress.com/.

##  Why use QualCoder?
**Qualcoder is free of charge.** Many qualitative analysis software requiring expensive one-time fees or monthly subscriptions. Not everyone can afford expensive fees.

**QualCoder is easy to use.** It has all you need to perform qualitative analysis without the complicated interfaces of some alternatives.

**QualCoder works offline.** Internet is not always available and QualCoder does not require internet to work.

**QualCoder is not tied to a computer.** If you change workplace you do not have to worry about being tied to your former workplace’s license or to buy a new license. QualCoder license allows you to use the software regardless of where you work or on what computer it is installed on.

**QualCoder is multi-platform.** It runs on Linux, Windows and Mac, this means that you do not have to worry if you change operating systems, and it also means you can collaborate with colleagues on different platforms.
**QualCoder relies on the community.** If you find a bug or have a feature request or feedback, write it on QualCoder’s page on github https://github.com/ccbogel/QualCoder.

**QualCoder is always improving.** QualCoder is actively developed meaning that newer, improved versions are released with improvements.

**QualCoder supports open standards.** QualCoder aims to support the REFI-QDA Standard, see https://www.qdasoftware.org/ You may exchange codebooks and projects with your colleagues even if they do not use QualCoder, as long as the software they use supports the REFI-QDA Standard. It means that you do not risk your data being unavailable. Note, as of December 2020 REFI-QDA Project is still experimental so there may be bugs. Further testing particularly for audio and video exports and imports and relatively-linked files is needed.

**QualCoder can be modified.** You can modify and adapt QualCoder to your needs, or if you do not how you ask someone to do it for you, as long as you release your changes to everyone. This also means you can copy the software and give it to your colleagues or students free of charge.

## Collaboration on a Qualcoder project

I get a few questions on how project collaboration works. So I have added this information on the first page of the wiki.
The first thing is that QualCoder is not set up to have multiple coders simultaneously working on  project. One person at a time must open the project and use the project.

The QualCoder project folder is a folder with a .qda ending. This folder contains sub-folders of files and a sqlite database file. You can zip the project folder and email (or transfer via removable media) the zipped project to another collaborator for them to work on the project. They unzip the folder, then open the project using QualCoder. 

You can have a second coder use the same project folder on the same computer, change the name in setting to the new coder's name (enter a new coder name and click the Apply button, or select from the drop down list) so they can work on the project under their name, especially if you need to do a coder comparison.

Please check the curernt coder's name in Files>Settings before doing any work. Codings in code text, code images, code A/V will only show the coded segments of the currently selected coder in Settings. So if **nothing** shows, change the coder name using the drop down box in Settings.

The coder name is 'default' when first using QualCoder. When opening another existing project, please make sure the coder name is set to the name you want to use by checking and updating the Settings before you do work on your project. When you are in any of the coding sections (coding text, images or A/V).

Do not use REFi-QDA Project export as a routine approach for collaboration when all coders are using QualCoder. Use the above approach instead. If you need to use open a project in different software (e.g. Taguette, NVivo, Atlas.ti, MAXQDA, Dedoose, Quirkos), only then you should use the REFI-QDA Project export. It is important to recognise that project features can be lost when transferring project between qualitative software using the REFI-QDA Project export.

21 June 2022 - I have stopped anyone from editing wikipages. Potential risks there.



