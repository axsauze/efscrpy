
# EFSCRA.py

This repo contains a small script that gets info from the ef portal into a csv file.

It builds a CSV with names, emails, pictures, questions, etc.

Requirements:

* Python 3.7
* Selenium
* PhantomJS or ChromeWebDriver

The recommended way to run is:

``` bash
    python3.7 efscra.py --username "USERNAME" --password "PASSWORD"
```

Remember to install requirements with:

``` bash
    pip3 install -r requirements.txt
```

## Chrome Webdriver

If you get an error with PhantomJS, with a message like "Screenshot: available via screen" make sure you install it. Alternatively you can just run it using the Chrome webdriver as outlined below.

In order to run you need to have Node and PhantomJS, or you need to download the chromedriver and specify the path with the --chrome flag:

``` bash
    python efscra.py --username "USERNAME" --password "PASSWORD" --chrome "PATH"
```

If you prefer to use the Chrome webdriver, you can specify the path to your driver with the --chrome flag.

Finally if your internet is quite slow, you can modify the waiting time with --waiting.