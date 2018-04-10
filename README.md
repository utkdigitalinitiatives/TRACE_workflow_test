# TRACE Workflow Test
This is a front end workflow testing script. This relies on [chrome webdriver](https://splinter.readthedocs.io/en/latest/drivers/chrome.html) & [Splinter](https://splinter.readthedocs.io/en/latest/)
It’s important to note that you also need to have Google Chrome installed in your machine.

## Install software and modules
Required: __chrome-driver__, [splinter](https://pypi.python.org/pypi/splinter), [lorem](https://pypi.python.org/pypi/loremipsum) <br/>


## Setup Environment
[WINDOWS 10 install Video Tutorial __Chrome-Driver__](https://youtu.be/dz59GsdvUF8)
* Create a folder `c:\webdrivers`
* System Properties > Advanced System Settings > Environment Variables > System Variables > Path > Edit > New
  * c:\webdrivers
  * Click OK/OK/OK
* Go to and download "Latest Release" > chromedriver_win32.zip
* Zip will extract to a single executable file 'chromedriver'
* Extract file to "c:\webdrivers/chromedriver"
* To test install open a command terminal and type `chromedriver` and it should start and press `ctrl c` to quit test.

### Install selenium (not recommended)
Chrome WebDriver is provided by Selenium2. To use it, you need to install Selenium2 via pip
```shell
$ pip install selenium
$ pip install splinter
$ pip install lorem
```

#### Fail safe way (recommended)
```terminal
$ pip install pipenv

# this installs the modules
$ pipenv sync

# To start the script in the pypenv and exit when complete
$ pipenv run python submit.py
```

#### To Run this app
```terminal
# To start this script
$ pipenv run python submit.py

```

## To modify submit.py
Use the 'SET config section'

```terminal
########### SET config section ###########

...

########### END SET config section ########
```

### SET config section

__supplimental_file__<br/>Set to current directory image file

__path_to_PDFs__<br/>This will randomly select any one of the PDFs in this directory and use it to submit.

__url__<br/>This is the URL for a page to trigger logging in. Using the 'user' page is ideal.

__how_many_submissions_to_submit__<br/>This is how many times you want the script to submit an ETD.

### Sometime the script with fail because of a timeout.
Just restart the script and it will work.
