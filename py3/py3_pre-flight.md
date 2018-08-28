## Python3 pre-flight

Below are instructions regarding installing things needed for general development with Python3 (including two example libraries). They include:

* [Xcode](https://developer.apple.com/xcode/) (Command Line Tools)
* [Homebrew](http://brew.sh/)
* [Python3](https://www.python.org/)
* [PyPI](https://pypi.python.org/pypi)
* [Jupyter](https://jupyter.org/index.html)
* [BeautifulSoup4](https://www.crummy.com/software/BeautifulSoup/)
* [Natural Language Toolkit](http://www.nltk.org/)


### Xcode / The Command Line Tools

Do you have **Xcode**? To check go to the terminal and execute `xcode-select -p`.

* If `/Applications/Xcode.app/Contents/Developer` (or something similar) appears as a response proceed to the next step.
* If anything else happens download and install `Xcode` from [here](https://itunes.apple.com/us/app/xcode/id497799835?mt=12) before moving on.

Enter `xcode-select --install` into the terminal, which should result in something like this:

![](/py3/imgs/xcode-select_install_cmnd_line_tools.png)

Click `Install` to download and install the **Xcode Command Line Tools** (it takes a while so maybe go make some food or get a cup of coffee or something).


### Homebrew

Copy and paste this code into the terminal and press `enter` to install [homebrew](http://brew.sh/):  `/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"`

If prompted, agree to the **Xcode** license

![](/py3/imgs/agree_to_xcode_license.png)

by executing `sudo xcodebuild -license` in the terminal.

Search to see if something is available on `homebrew` with `search`. For example:  `brew search python3`


### Python3

To install **Python3** execute `brew install python3` in the terminal.


### PyPI

**PyPi** is frequently referred to as `pip`. It is used to manage **Python** library installations and ships with **Python3** when installed via **Homebrew**. The command to use it is `pip3`, **not** `pip`.

Search for something on `pip3` with the `search` command. For example: `pip3 search jupyter`


### Jupyter

Install **Jupyter** via `pip3` as follows:
1. `pip3 install --upgrade pip`
2. `pip3 install jupyter`

Executing `jupyter notebook` in the terminal starts the [IDE](https://en.wikipedia.org/wiki/Integrated_development_environment).

![](/py3/imgs/jupyterhome.png)

On the **Jupyter** homepage click `New` and select **Python3**. This will create and open an **iPython Notebook** file.

![](/py3/imgs/pyjupyternotebook.png)

Click `File`, select `Save As` and then name the file. Next click `File` and select `Close and Halt` to exit.

When you return to the **Jupyter** homepage you should see the **iPython Notebook** file (`.ipynb`) that you just saved.

![](/py3/imgs/jupyteripynb.png)


### BeautifulSoup4

`pip3 install beautifulsoup4`

### lxml

`pip3 install lxml`


### Natural Language Toolkit

`sudo pip3 install -U nltk`

Confirm that it works with the following steps (all in the terminal):

1. `ipython3`
2. `import nltk`
3. `nltk.` and then hit the `TAB` key on your keyboard


### NLTK Things

Run **Jupyter**, navigate to the file you created earlier, import the **NLTK** library, then run the downloader in the following steps:

1. `jupyter notebook`
2. Navigate to the file, open it
3. `import nltk`
4. `nltk.download()`

A new terminal window will open that looks like the image below. Select `book` and click `Download`:

![](/py3/imgs/nltk_downloader_book.png)
