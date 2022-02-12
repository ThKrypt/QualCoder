# QualCoder Installation and running instructions

## INSTALLATION 

### Prerequisites
You will need to have a python3.6 or newer version installed and a 64 bit VLC player installed. 

### Windows

Install  [VLC](https://www.videolan.org/vlc/download-windows.html) or from the Windows Store. 

The 2.8 Release contains an exe file (created on Windows 10, 64 bit). Double-click to run. This does work on older Windows versions (e.g. Win 7).

**Alternatively:**

1. Download the QualCoder software from: https://github.com/ccbogel/QualCoder. This is the newest, but not yet officially released code. Alternatively, choose the most recent release. Click the green button "Code", and then "Download ZIP". Then, unpack the file in a selected place (e.g. desktop).

2. Download and install the Python programming language. The minimum version for QualCoder is 3.6.  [Python3](https://www.python.org/downloads/). Download the file (at the bottom of the web site) "Windows installer (64-bit)"
IMPORTANT: in the first window of the installation mark the option "Add Python to PATH"

3. Install python modules from command. Type "cmd" in the Windows Start search engine, and click on the black software "cmd.exe" - the command console for Windows. In the console type or paste, using the right-click context menu (ctrl+v does not work) the following:

`py -m pip install wheel pyqt5 lxml Pillow ebooklib ply chardet pdfminer.six openpyxl pydub SpeechRecognition`

 Wait, until all modules are installed .
 
4. Build and install Qualcoder, from the downloaded folder type

`py setup.py install`

The `py` command uses the most recent installed version of python. You can use a specific version on your Windows, if you have many python versions installed, e.g. `py -3.8`  See discussion here: [Difference between py and python](https://stackoverflow.com/questions/50896496/what-is-the-difference-between-py-and-python-in-the-terminal)

5. Run QualCoder from cmd.exe
Move to the QualCoder-master folder, or (for a release, e.g.) the QualCoder-2.8 folder, then type 

`py -m qualcoder`

Alternately, run by double-click. Open the QualCoder-master\qualcoder folder. Double-click the \_\_main\_\_.py file to run. You can make a shortcut to this file and keep the shortcut on the desktop.

### Debian/Ubuntu Linux

It is best to run QualCoder inside a python virtual environment, so that the system install python modules do not clash and cause problems. I have added the additional code to do this here.

Install venv I am using python3.9 you can choose another recent version if you prefer. 

`sudo apt install python3.9-venv`

Download and unzip the Qualcoder folder.

Open a terminal and move (cd) into that folder. You should be inside the QualCoder-master folder or if using a release, e.g. the Qualcoder-2.9 folder. Inside the QualCoder-master folder: 

`python3.9 -m venv qualcoder`

Activate venv, this changes the command prompt display using (brackets): (qualcoder) 
Note: To exit venv type deactivate 

`source qualcoder/bin/activate`

Install the required python modules:

`pip install lxml ply six pdfminer chardet pyqt5 pillow pdfminer.six openpyxl ebooklib pydub SpeechRecognition`

Install QualCoder (the dot is important):

`python3 -m pip install .`

You may get a warning which can be ignored: WARNING: Building wheel for Qualcoder failed

To run type

`qualcoder`

After all this is done, you can deactivate to exit the virtual environment. At any time to start QualCoder in the virtual environment, cd to the Qualcoder-master folder (or Qualcoder-2.9 release folder), 

Then type: `source qualcoder/bin/activate` 

Then type `qualcoder`


OLDER instructions below that can affect system installed python modules. It is better to use the virtual environment shown above.
1. Install  modules from the command line

`sudo apt install python3-pip python3-lxml python3-ply python3-six python3-pdfminer python3-chardet python3-pyqt5 python3-pillow`

2. Install additional modules

`sudo python3 -m pip install pdfminer.six openpyxl ebooklib pydub SpeechRecognition`

3. Building and install QualCoder, from the downloaded folder (Qualcoder-master or a release e.g. QualCoder-2.8) type

`sudo python3 setup.py install`

4. To run type

`qualcoder`


### Arch/Manjaro Linux

Please see the Debian instructions above to run QualCoder in a virtual environment. I do not have an Arch/Manjaro distribution to test this.

1. Install modules from the command line

`sudo pacman -S python python-lxml python-ply python-six python-pdfminer python-chardet python-pyqt5 python-pillow python-pip`

2. Install additional python modules

`sudo python3 -m pip install pdfminer.six openpyxl ebooklib pydub SpeechRecognition`

If success, all requirements are satisfied.

3. Build and install QualCoder, from the downloaded folder (Qualcoder-master or a release e.g. QualCoder-2.8) type

`sudo python3 setup.py install`

4. To run type:

`qualcoder`

### Fedora/CentOS/RHEL linux

Please see the Debian instructions above to run QualCoder in a virtual environment. I do not have a Fedora/CentOS/RHEL distribution to test this.

Retrieve the current package code from this repository

`git clone https://github.com/ccbogel/QualCoder.git`

Make `install_fedora.sh` executable (`chmod +x install_fedora.sh`) and run the `./install_fedora.sh` script from the terminal. Make sure the qualcoder folder is in the same directory as the install.sh script (i.e. as it appears when you download the QualCoder-master folder). The script is for python version 3.9.

This script installs the dependencies using dnf and the ebook libraries with a work-around, specified at https://github.com/ccbogel/QualCoder/issues/72#issuecomment-695962784.

Fedora uses wayland with does not work well with the Qt graphical interface (for now). I suggest you also install xwayland.

### MacOS

1) Install recent versions of [Python3](https://www.python.org/downloads/) and [VLC](https://www.videolan.org/vlc/).

2) Download the latest release "Source code" version in ZIP format, from the releases section of the project here on Github: https://github.com/ccbogel/QualCoder/releases/tag/2.8 and extract it into /Applications

3) Open the Terminal app (or any other command shell)

4) Install PIP (if not yet installed, try typing `pip3 --version` and hit ENTER) 

```sh
curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py
python3 get-pip.py
```

-> You should now be able to run `pip3` as above.

5) Install Python dependency modules using `pip`:

(you might already have them, don't do this again if you just update QualCoder to a newer version)

```sh
pip install pyqt5 lxml pillow six ebooklib ply chardet pdfminer.six openpyxl pydub SpeechRecognition
```

6) Install system dependencies using Homebrew (aka `brew`) 

6.1) Install `brew` if do not already have it (try typing `brew` and hit ENTER):

* Follow instructions here about installing Homebrew on your macOS: https://brew.sh/

6.2) Install QPDF package (needed to deal with PDF files) using Homebrew package manager:

```sh
brew install qpdf
```

From the QualCoder-Master directory run the setup script:

`python3 setup.py install`


Assuming you downloaded the 2.8 version. You can now run with:

```
python3 /applications/QualCoder-2.8/qualcoder/__main__.py
```

Alternative commands to run QualCoder (Suggestions):

From any directory:

`qualcoder`

From the QualCoder-Master directory:

`python -m qualcoder`

or

`python qualcoder/__main__.py`

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