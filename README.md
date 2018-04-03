# TRACE Workflow Test
This is a front end workflow testing script. This relies on [chrome webdriver](https://splinter.readthedocs.io/en/latest/drivers/chrome.html) & [Splinter](https://splinter.readthedocs.io/en/latest/)

## Install modules
```terminal
pip install splinter random lorem
```

## To modify
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
