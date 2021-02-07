# Welcome to the QualCoder wiki

![QualCoder Icon](https://qualcoder.files.wordpress.com/2019/01/qualcoder.png?w=500)

## What is QualCoder?
QualCoder is free, open source software for qualitative data analysis. 
With QualCoder you can code text, images, audio and video, write journal notes and memos. You can categorise codes into a tree-like hierarchical categorisation scheme. Coding for audio and video requires the VLC media player.
Coder comparison reports can be generated for text coding using the Cohen’s Kappa statistic. A graph displaying codes and categories can be generated to visualise the coding hierarchy. Most reports can be exported at html, open document text (ODT) or as plain text files.
QualCoder is written in python 3 (version 3.6 and up) using Qt5 for the graphical interface. A Sqlite database is used to store the coding data.
There is also a wordpress site for QualCoder at https://qualcoder.wordpress.com/.

###  Why use QualCoder?
Firstly, QualCoder is free. You do not need to pay for a commercial software license. QualCoder is easy to use and contains the core functionalities required for qualitative analysis. You use Linux. QualCoder has been developed on Linux and also works on Windows and MacOS. There are many Free/Libre Open Source Software (FLOSS) supporters who are willing to use and support FLOSS development.

## Downloading files and dependencies
Download the latest QualCoder from GitHub: https://github.com/ccbogel/QualCoder. Unzip the folder. The main program code is in the QualCoder folder. The Examples folder contains some example files which can be loaded into a test QualCoder project. 

**Microsoft Windows**

You will need to download and install Python 3 (the minimum version is python 3.6, or a newer version). Then install python modules. Python 3 releases can be obtained here: https://www.python.org/downloads/windows/. Finally, you need to have the VLC media player installed. Please ensure that the Python and VLC downloads are in the same architecture – that is – 32 bit or 64 bit for both. Otherwise QualCoder will not work.You can get this from the Windows Store or from their website: https://www.videolan.org/vlc/download-windows.html 
Once a Python 3 release is installed you should be able to install the modules using the following commands in the Windows Command prompt (The prompt is under Windows System):

`python -m pip install pyqt5 lxml Pillow ebooklib ply chardet pdfminer.six openpyxl`

To run QualCoder - double click on the qualcoder.py file which is located inside the qualcoder directory. You can make a shortcut to this file on the Desktop.

**Linux Ubuntu/Debian**

QualCoder can be installed using the latest Debian file found here: https://github.com/ccbogel/QualCoder-Debians

If you want to install using the _install.sh_ script, follow these instructions to create a program launcher:
Go to your downloads folder. The example script below assumes you have downloaded the QualCoder-master.zip. Unzip QualCoder-master.zip. Open the uzipped folder and make the _install.sh_ script executable.  Open a terminal and type the following to install QualCoder:

cd Downloads/QualCoder-master

Run the _install.sh_ file. The install process will ask for your permission to install QualCoder into the /usr/share directory. It will also download the additional dependencies.

`./install.sh`

**Linux Fedora/CentOS/RHEL**

Retrieve the current package code from this repository

`git clone https://github.com/ccbogel/QualCoder.git`

Install dependencies

`sudo dnf install python3-pip python3-lxml python3-ply python3-six python3-chardet python3-qt5 python3-pillow`

QualCoder uses an Ebook library that you can currently install via a work-around, specified at https://github.com/ccbogel/QualCoder/issues/72#issuecomment-695962784 

The UNTESTED install_fedora.sh should install the dependencies and a desktop start icon for Fedora. The script is for python version 3.8.

**MacOS**

Install Python3 (minimum version is 3.6) and VLC. 

Download Qualcoder-master Zip file and copy it into /Applications
In a Terminal run these commands to use (for example) python 3.9:
Download Qualcoder-master Zip file and copy it into /Applications

    Open the Terminal app (or any other command shell)

    Install PIP (if not yet installed, try typing pip3 --version and hit ENTER)

`curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py`
`python3 get-pip.py`

-> You should now be able to run pip3 as above.

    Install Python dependency modules using pip:

(you might already have them, don't do this again if you just update QualCoder to a newer version)

`pip install pyqt5 lxml pillow six ebooklib ply chardet pdfminer.six openpyxl`

    Install system dependencies using Homebrew (aka brew)

4.1) Install brew if do not already have it (try typing brew and hit ENTER):

    Follow instructions here about installing Homebrew on your macOS: https://brew.sh/

4.2) Install QPDF package (needed to deal with PDF files) using Homebrew package manager:

`brew install qpdf`

    Finally, install QualCoder, anywhere you want on your system, most likely somewhere in your user home directory.

5.1) Download the latest "Source code" version in TAR/GZIP format, from the releases section of the project here on Github: https://github.com/ccbogel/QualCoder/releases

Assuming here after, you saved the archive of version 2.2 in your "Downloads" folder, and we would install directly in your "home" (/Users/YourName/ or ~ for shortcut).

For example:

`cd ~`
`tar -xzvf ~/Downloads/QualCoder-2.2.tar.gz`

The last should have extracted all the archive into ~/QualCoder-2.2.

You can now run with:

`python3 ~/QualCoder-2.2/qualcoder/qualcoder.py`

Remember: You can install it anywhere you want, so the path above depends on where you extracted the archive before ;)

Another option to run Qualcoder is shown here: https://www.maketecheasier.com/run-python-script-in-mac/. This means you can right-click on the qualcoder.py file and open with --> python launcher. You can make an alias to the file and place it on your desktop.

Another option to install on Mac:

Open the Terminal App and move to the unzipped Qualcoder-Master directory, then run the following command:

`python3 setup.py py2app`


# Starting QualCoder

### Linux
If you have successfully installed the debian package or sucessfully run the install.sh script there will be a program launcher. Double-click to start.

Alternatively, using the terminal, move to the inner QualCoder folder and open the qualcoder.py file:

`python3 qualcoder.py`

### Windows
In Windows create a shortcut to the qualcoder.py file and double click to open. Alternatively, using the command prompt, move to the directory and open the qualcoder.py file:

`python3 qualcoder.py`

### Mac OS
There is no desktop icon launch right now for QualCoder. Open a new Terminal window in the directory and launch with 
`python3 qualcoder.py`

## Backups

I recommend that you make a backup before doing any substantial changes, such as reorganising codes and categories. QualCoder does perform hourly backups (keeping the most recent five) if backups is set in the settings.


Edition August 2020 Author: Colin Curtain ccbogel@hotmail.com

# Notice

**Copyright Notice**

The MIT License (MIT)

Copyright (c) 2020 Colin Curtain
Permission is hereby granted, free of
 charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.