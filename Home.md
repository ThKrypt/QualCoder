# Welcome to the QualCoder wiki

![QualCoder Icon](https://qualcoder.files.wordpress.com/2019/01/qualcoder.png?w=500)

## What is QualCoder?
QualCoder is free, open source software for qualitative data analysis. 
With QualCoder you can code text, images, audio and video, write journal notes and memos. You can categorise codes into a tree-like hierarchical categorisation scheme. Coding for audio and video requires the VLC media player.
Coder comparison reports can be generated for text coding using the Cohen’s Kappa statistic. A graph displaying codes and categories can be generated to visualise the coding hierarchy. Most reports can be exported at html, open document text (ODT) or as plain text files.
QualCoder is written in python 3 using Qt5 for the graphical interface. A Sqlite database is used to store the coding data.
There is also a wordpress site for QualCoder at https://qualcoder.wordpress.com/.

###  Why use QualCoder?
Firstly, QualCoder is free. You do not need to pay for a commercial software license. QualCoder is easy to use and contains the core functionalities required for qualitative analysis. You use Linux. QualCoder has been developed on Linux and also works on Windows and MacOS. There are many Free/Libre Open Source Software (FLOSS) supporters who are willing to use and support FLOSS development.

## Downloading files and dependencies
Download the latest QualCoder from GitHub: https://github.com/ccbogel/QualCoder. Unzip the folder. The main program code is in the QualCoder folder. The Examples folder contains some example files which can be loaded into a test QualCoder project. 

**Microsoft Windows**

You will need to download and install Python 3. Then install PyQt5, lxml and Pillow modules. A Python 3 release can be obtained here: https://www.python.org/downloads/windows/. Finally, you need to have the VLC media player installed. Please ensure that the Python and VLC downloads are in the same architecture – that is – 32 bit or 64 bit for both. Otherwise QualCoder will not work.You can get this from the Windows Store or from their website: https://www.videolan.org/vlc/download-windows.html 
Once a Python 3 release is installed you should be able to install the modules using the following commands in the Windows Command prompt (The prompt is under Windows System):

`python -m pip install pyqt5 lxml Pillow ebooklib ply chardet click pikepdf pdfminer.six`

To run QualCoder - double click on the qualcoder.py file which is located inside the qualcoder directory. You can make a shortcut to this file on the Desktop.

**Linux**

QualCoder can be installed using the latest Debian file found here: https://github.com/ccbogel/QualCoder-Debians

If you want to install using the _install.sh_ script, follow these instructions to create a program launcher:
Go to your downloads folder. The example script below assumes you have downloaded the QualCoder-master.zip. Unzip QualCoder-master.zip. Open the uzipped folder and make the _install.sh_ script executable.  Open a terminal and type the following to install QualCoder:

cd Downloads/QualCoder-master

Run the _install.sh_ file. The install process will ask for your permission to install QualCoder into the /usr/share directory. It will also download the additional dependencies.

`./install.sh`


**MacOS**

Install Python3 and VLC. Install the Python dependencies using pip:

`pip install pyqt5 lxml pillow sixebooklib ply chardet click pikepdf pdfminer.six`

There is no desktop icon launch right now for QualCoder. Open a new Terminal window in the directory and launch with python qualcoder.py.

# Starting QualCoder

### Linux
If you have successfully installed the debian package or sucessfully run the install.sh script there will be a program launcher. Double-click to start.

Alternatively, using the terminal, move to the inner QualCoder folder and open the qualcoder.py file:

`python3 qualcoder.py`

### Windows
In Windows create a shortcut to the qualcoder.py file and double click to open. Alternatively, using the command prompt, move to the directory and open the qualcoder.py file:

`python3 qualcoder.py`

### Mac OS
There is no desktop icon launch right now for QualCoder. Open a new Terminal window in the directory and launch with python qualcoder.py.

## Backups

QualCoder does make a backup of a project when the project is first opened. I recommend that you make a backup before doing any substantial changes, such as reorganising codes and categories.


Edition August 2019 Author: Colin Curtain ccbogel@hotmail.com

**Copyright Notice**
The MIT License (MIT)
Copyright (c) 2019 Colin Curtain
Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.