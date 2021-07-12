# QualCoder Installation and running instructions

![QualCoder Icon](https://qualcoder.files.wordpress.com/2019/01/qualcoder.png?w=500)

## Downloading files and dependencies
Download the latest Qualcoder release from https://github.com/ccbogel/QualCoder/releases or the latest development from https://github.com/ccbogel/QualCoder. Unzip the folder. The main program code is in the inner qualcoder folder. The Examples folder contains some example files which can be loaded into a test QualCoder project. 

## Microsoft Windows

**For ease of use. The QualCoder 2.7 release has an exe for Windows 64 bit computers: https://github.com/ccbogel/QualCoder/releases/tag/2.7**

**Please ensure you have the VLC installed as well, for QualCoder to work. The QualCoder exe file bundles up all the python modules needed to run.**

Alternative installation instructions for Windows:

Download the QualCoder software from: https://github.com/ccbogel/QualCoder. This is the newest, but not yet officially released, version of code. Alternatively, choose the most recent release. Click the green button "Code", and then "Download ZIP". Then, unpack the file in a selected place (e.g. desktop).

Open the unpacked folder "QualCoder-master", then open the inner folder "qualcoder" and make a shortcut of the file "qualcoder.py" on the desktop - for easier access. This file is the starting file for running software.

The software is written in Python and does not have an exe file for Windows. Download and install the Python programming language. The minimum version is 3.6. Newer is better, e.g. 3.8.7 (https://www.python.org/downloads/release/python-387/). Download the file (at the bottom of the web site) "Windows installer (64-bit)" (or 32-bit if you have an older system) and install Python.

IMORTANT: in the first window of the python installation mark the option "Add Python 3.8 to PATH" - it makes the last step easier.

Install extra modules to Python. Type the letters "cmd" in the Windows Start searching engine, and click on the black software "cmd.exe" - this is the command console for Windows. In the console paste, using the right-click context menu (ctrl+v does not work) the following:

`py -m pip install pyqt5 lxml Pillow ebooklib ply chardet pdfminer.six openpyxl py2exe`

(You can skip the py2exe instruction for now, it is not actively used yet)

Then click enter. Wait, until all modules are installed (the command phrase should be again visible: "C:\Users[Your Windows account name]> or similar).


### Running for 2.7 and higher releases:

Run QualCoder from cmd.exe
Move (cd) to the QualCoder-Master folder, or the release folder if you downloaded the release (e.g. QualCoder-2.7 folder). 
Then type:

`py -m qualcoder`

Or running and hiding the command line box:

`C:\Windows\pyw.exe -m qualcoder`

Run by mouse double-click
Open the QualCoder-master\qualcoder folder. Double-click the \_\_main\_\_.py file to run. You can make a shortcut to this file and keep the shortcut on the desktop.

### Running for 2.5 and lower releases

To run QualCoder - double click on the qualcoder.py file which is located in the inner qualcoder folder. You can make a shortcut to this file on the Desktop.

## Linux Ubuntu/Debian

### Install and running for 2.7 and higher releases

Install these modules from the terminal

`sudo apt install python3-lxml python3-ply python3-six python3-pdfminer python3-chardet python3-qt5 python3-pillow`

On some Linux versions you will need to install pip

`sudo apt install python3-pip`

You also need to run this command from the terminal:

`sudo python3 -m pip install pdfminer.six openpyxl ebooklib`

Install QualCoder by moving to the QualCoder-Master folder or the release folder, e.g. QualCoder-2.7:

`sudo python3 setup.py install`

Running, anytime the terminal is opened:

`qualcoder`

### For releases 2.5 and earlier (Ubuntu, Debian)

QualCoder can be installed using the latest Debian file found here: https://github.com/ccbogel/QualCoder-Debians

If you want to install using the _install.sh_ script, follow these instructions to create a program launcher:
Go to your downloads folder. The example script below assumes you have downloaded the QualCoder-master.zip. Unzip QualCoder-master.zip. Open the uzipped folder and make the _install.sh_ script executable.  Open a terminal and type the following to install QualCoder:

cd Downloads/QualCoder-master

Run the _install.sh_ file. The install process will ask for your permission to install QualCoder into the /usr/share directory. It will also download the additional dependencies.

`./install.sh`

## Linux Fedora/CentOS/RHEL

### For releases 2.5 and earlier. Retrieve the current package code from this repository.

`git clone https://github.com/ccbogel/QualCoder.git`

Install dependencies

`sudo dnf install python3-pip python3-lxml python3-ply python3-pdfminer python3-six python3-chardet python3-qt5 python3-pillow`

QualCoder uses an Ebook library that you can currently install via a work-around, specified at https://github.com/ccbogel/QualCoder/issues/72#issuecomment-695962784 

The UNTESTED install_fedora.sh should install the dependencies and a desktop start icon for Fedora. The script is for python version 3.8.

Fedora uses wayland with does not work well with the Qt graphical interface (for now). I suggest you also install xwayland.

### Running 2.7 and newer releases (untested).

`sudo dnf install python3-pip python3-lxml python3-ply python3-pdfminer python3-six python3-chardet python3-qt5 python3-pillow`

QualCoder uses an Ebook library that you can currently install via a work-around, specified at https://github.com/ccbogel/QualCoder/issues/72#issuecomment-695962784 

Move to the Qualcoder-master folder (or the release folder, if this was downloaded, e.g. QualCoder-2.7) and run:

`python3 setup.py install`

Run by typing:

`qualcoder`

## MacOS

1) Install recent versions of [Python3](https://www.python.org/downloads/) and [VLC](https://www.videolan.org/vlc/).

2) Download the latest release "Source code" version in ZIP format, from the releases section of the project here on Github: https://github.com/ccbogel/QualCoder/releasesDownload and extract it into /Applications

3) Open the Terminal app (or any other command shell)

4) Install PIP (if not yet installed, try typing `pip3 --version` and hit ENTER) 

```sh
curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py
python3 get-pip.py
```

-> You should now be able to run `pip3` as above.

5) Install Python dependency modules using `pip`:

You might already have the modules. You do not need to do this again if you update QualCoder to a newer version.

```sh
pip install pyqt5 lxml pillow six ebooklib ply chardet pdfminer.six openpyxl
```


6) Note step 6 is not essential on Mac, but may be useful of you are trying to import encrypted pdf text.
Install system dependencies using Homebrew (aka `brew`) 

6.1) Install `brew` if do not already have it (try typing `brew` and hit ENTER):

* Follow instructions here about installing Homebrew on your macOS: https://brew.sh/

6.2) Install QPDF package (needed to deal with PDF files) using Homebrew package manager:

```sh
brew install qpdf
```


### Running the 2.5 version. You can now run with:

```
python3 /applications/QualCoder-2.5/qualcoder/qualcoder.py
```

### Running the 2.6 and higher versions (untested):
python3 /applications/QualCoder-2.5/qualcoder/\_\_main\_\_.py

You can install QualCoder anywhere you want, so the path above depends on where you extracted the archive.

Another option to run Qualcoder is shown here: [https://www.maketecheasier.com/run-python-script-in-mac/](https://www.maketecheasier.com/run-python-script-in-mac/). This means you can right-click on the qualcoder.py file and open with --> python launcher. 
You can make an alias to the file and place it on your desktop.

**Another option to install on Mac:**

Open the Terminal App and move to the unzipped Qualcoder-Master directory, then run the following commands:

`pip install -U py2app`  or for a system installation of python `sudo pip install -U py2app`

`python3 setup.py py2app` 


## Backups

I recommend that you make a backup before doing any substantial changes, such as reorganising codes and categories. QualCoder does perform hourly backups (keeping the most recent five) if backups is set in the settings.



# Notice

**Copyright Notice**

The MIT License (MIT)

Copyright (c) 2021 Colin Curtain
Permission is hereby granted, free of
 charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.