# Rikaitan MeCab Installer

Installs the files required to run [MeCab](https://taku910.github.io/) in [Rikaitan](https://github.com/Ajatt-Tools/rikaitan/).
Python and MeCab have to be installed separately.

## Installation

If you are running Mac, first install [Homebrew](https://brew.sh/), as it is used to install the dependencies.

1. Install Python
    - **Windows**: https://www.python.org/downloads/
    - **Mac**: Run `brew install python3`
    - **Linux**: Python is usually included with a Linux distribution.
1. Install MeCab
    - **Windows**: https://taku910.github.io/mecab/#download (mecab-x.xxx.exe:ダウンロード)
    - **Mac**: run `brew install mecab`
    - **Linux**: package managers usually include MeCab. You don't need to install a dictionary package from the package manager, this script downloads the required dictionaries for you.
1. [Download](https://github.com/Ajatt-Tools/rikaitan-mecab-installer/archive/master.zip) and extract this repository to the location where you wish to install the files. `~/Downloads` might not be the best place, as the dictionary files are stored in the same directory.
1. Run `install_mecab_for_rikaitan.py` using Python and follow the instructions.
2. Go to the Rikaitan settings page in the browser you selected.
3. Enable advanced options by clicking the toggle switch in the bottom left corner.
4. Go to `Text Parsing`.
5. Enable `Parse sentences using MeCab`.
6. To check if it's installed correctly, click the `More...` button and select `Test`. If it returns "Connection was successful", MeCab is now installed for Rikaitan.

Some things to note:
- If you try to run the installer for use on multiple browsers, it will not work. Only one browser can use the MeCab for Rikaitan installation.
- If you wish to use MeCab on another browser, close the browser that has MeCab for Rikaitan installed. If you do not do this, you will get a `Permission denied` error when running the script.
- If you ran the script but clicking the `Test` button in the Settings page displays `Could not connect to native MeCab component`, try to close and reopen your browser. If that does not work, try to run the script without the browser running. If you have any questions, you can contact me on Matrix with the username starxeras.

![demo video](demo.gif)
*Demo video using Linux*

You can move the install directory later, but you have to run the install again if you do that.
