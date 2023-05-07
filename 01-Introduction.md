# QualCoder Installation and running instructions

## INSTALLATION 

### Prerequisites
For versions 3.2 and newer, VLC is optional, but you will need it installed if you need to do any audio/video coding. Optionally, install ffmpeg for speech to text and waveform display, see https://phoenixnap.com/kb/ffmpeg-windows..

### Windows

**Use the exe**

Current releases contain an exe file (created on Windows 10, 64 bit). Double-click to run.

**Alternatively install from source**

Seriously consider using a virtual environment (commands in point 6 below). Not using a virtual environment may affect other python software you may have installed.

1. Download and install the Python programming language. The minimum version for QualCoder is 3.7. I recommend 3.10 for now. [Python3](https://www.python.org/downloads/). Download the file (at the bottom of the web site) "Windows installer (64-bit)"
IMPORTANT: in the first window of the installation mark the option "Add Python to PATH"

2. Download the QualCoder software from: https://github.com/ccbogel/QualCoder from the Green Code button. This is the newest, but not yet officially released code. Click the green button "Code", and then "Download ZIP". Alternatively, choose the most recent release zip, see right hand side of this page for the link to Releases.

3. Unzip the folder to a location (e.g. downloads). (Tip, remove the doubled up folder extraction QualCoder-master\QualCoder-master when asked where to extract. Just QualCoder-master).

4. Use the Windows command prompt. Type "cmd" in the Windows Start search engine, and click on the black software "cmd.exe" - the command console for Windows. In the console type or paste, using the right-click mouse copy and paste (ctrl+v does not work)

5. In the command prompt, move (using the `cd` command) into the QualCoder folder. You should be inside the QualCoder-master folder or if using a release (the Qualcoder-3.2 folder). e.g.

`cd Downloads\QualCoder-master`

6. Install and activate the virtual environment. This step can be skipped, but I recommend you do not skip it.

`pip install virtualenv`

Create a virtual environment called env.

`virtualenv env`

Activate the virtual environment, this changes the command prompt display using (brackets): (env)

`env\Scripts\activate.bat`

7. Install python modules. Type the following:

`py -m pip install --upgrade pip`

`py -m pip install wheel pyqt6 chardet ebooklib openpyxl Pillow ply pdfminer.six pandas plotly pydub python-vlc rispy SpeechRecognition xmlschema`

Wait, until all modules are installed .

8. Install QualCoder, from the downloaded folder type:

`py -m pip install .`

The py command uses the most recent installed version of python. You can use a specific version on your Windows, if you have many python versions installed, e.g. py -3.10 See discussion here: [Difference between py and python](https://stackoverflow.com/questions/50896496/what-is-the-difference-between-py-and-python-in-the-terminal)

9. Run QualCoder from the command prompt:

`py -m qualcoder`

10. If running QualCoder in a virtual environment, to exit the virtual environment type:

`deactivate`

The command prompt will then remomove the (env) wording.

11. To start QualCoder again:

If you are not using virtual environment, as long as you are in the same drive letter, eg C:

`py -m qualcoder`

If you are using a virtual environment:

`cd` to the Qualcoder-master (or Qualcoder release folder), then type:

`env\Scripts\activate.bat`

`py -m qualcoder`

### Debian/Ubuntu Linux

There is an executable file in the releases page for Ubuntu 22.04 for the 3.2 release. Download and double click to run.

Alternatively, run QualCoder inside a python virtual environment, so that the system installed python modules do not clash and cause problems. I have added the additional code to do this here.

Install venv I am using python3.10 you can choose another recent version if you prefer. 

`sudo apt install python3.10-venv`

Download and unzip the Qualcoder folder.

Open a terminal and move (cd) into that folder. You should be inside the QualCoder-master folder or if using a release, e.g. the Qualcoder-3.0 folder. Inside the QualCoder-master folder: 

`python3.10 -m venv qualcoder`

Activate venv, this changes the command prompt display using (brackets): (qualcoder) 
Note: To exit venv type deactivate 

`source qualcoder/bin/activate`

Upgrade pip before installing the modules:

`pip install --upgrade pip`

Install the required python modules:

`pip install chardet ebooklib openpyxl pandas ply pdfminer pyqt6 pillow pdfminer.six plotly pydub python-vlc six SpeechRecognition xmlschema`

Install QualCoder (the dot is important):

`python3 -m pip install .`

To run type

`qualcoder`

After all this is done, you can deactivate to exit the virtual environment. At any time to start QualCoder in the virtual environment, cd to the Qualcoder-master folder (or Qualcoder-3.0 release folder), 

Then type: `source qualcoder/bin/activate` 

Then type `qualcoder`


### Arch/Manjaro Linux

Please consider the Debian instructions above to run QualCoder in a virtual environment.

1. Install modules from the command line

`sudo pacman -S python python-chardet python-openpyxl python-pillow python-ply python-pyqt6 python-pip`

2. Install additional python modules

`sudo python3 -m pip install ebooklib pdfminer.six pandas plotly pydub python-vlc SpeechRecognition`

If success, all requirements are satisfied.

3. Build and install QualCoder, from the downloaded folder (Qualcoder-master or a release e.g. QualCoder-3.1) type

`sudo python3 -m pip install .`

4. To run type:

`qualcoder`

Or install from AUR as follows:

`yay -S qualcoder`

### Fedora/CentOS/RHEL linux

Please consider the Debian instructions above to run QualCoder in a virtual environment. I do not have a Fedora/CentOS/RHEL distribution to test this.

Retrieve the current package code from this repository

`git clone https://github.com/ccbogel/QualCoder.git`

Make `install_fedora.sh` executable (`chmod +x install_fedora.sh`) and run the `./install_fedora.sh` script from the terminal. Make sure the qualcoder folder is in the same directory as the install.sh script (i.e. as it appears when you download the QualCoder-master folder). The script is for python version 3.9.

This script installs the dependencies using dnf and the ebook libraries with a work-around, specified at https://github.com/ccbogel/QualCoder/issues/72#issuecomment-695962784.

Fedora uses wayland with does not work well with the Qt graphical interface (for now). I suggest you also install xwayland.

### MacOS

1) Install recent versions of [Python3](https://www.python.org/downloads/) and [VLC](https://www.videolan.org/vlc/).

2) Download the latest release "Source code" version in ZIP format, from the releases section of the project here on GitHub: https://github.com/ccbogel/QualCoder/releases/tag/3.2 and extract it into /Applications

3) Open the Terminal app (or any other command shell)

4) Install PIP (if not yet installed, try typing `pip3 --version` and hit ENTER) 

```sh
curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py
python3 get-pip.py
```

-> You should now be able to run `pip3` as above.

5) Install Python dependency modules using `pip`:

```sh
pip install pyqt6 chardet ebooklib pillow ply pdfminer.six openpyxl pandas plotly pydub python-vlc six SpeechRecognition xmlschema
```

From the QualCoder-Master directory run the setup script:

6) `python3 -m pip install .`


Assuming you downloaded the 3.2 version. You can now run with:

```
python3 /applications/QualCoder-3.2/qualcoder/__main__.py
```

Alternative commands to run QualCoder (Suggestions):

From any directory:

`qualcoder`

From the QualCoder-Master directory:

`python3 -m qualcoder`

You can install QualCoder anywhere you want, so the path above depends on where you extracted the archive.

Another option to run Qualcoder is shown here: [https://www.maketecheasier.com/run-python-script-in-mac/](https://www.maketecheasier.com/run-python-script-in-mac/). This means you can right-click on the qualcoder.py file and open with --> python launcher. 
You can make an alias to the file and place it on your desktop.

**Another option to install on Mac:**

Open the Terminal App and move to the unzipped Qualcoder-Master directory, then run the following commands:

`pip3 install -U py2app`  or for a system installation of python `sudo pip3 install -U py2app`

`python3 setup.py py2app` 
## Backups

I recommend that you make a backup before doing any substantial changes, such as reorganising codes and categories. QualCoder does perform hourly backups (keeping the most recent five) if backups is set in the settings.



# Notice

**Copyright Notice**

The MIT License (MIT)

Copyright (c) 2023 Colin Curtain
Permission is hereby granted, free of
 charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.