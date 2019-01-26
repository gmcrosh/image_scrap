# Example image scrapper

Scraps image off of google images for training a neural network. The example only downloads images that are labeled for [reuse](https://support.google.com/websearch/answer/29508?hl=en).

## Setup

The code requires chrome and chrome driver. These are driven by selenium, with low usage this will not trigger any bot detection.

### Installing chrome and chrome driver
```
wget https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb
sudo dpkg -i google-chrome-stable_current_amd64.deb
apt-get install -f
wget https://chromedriver.storage.googleapis.com/2.45/chromedriver_linux64.zip
apt-get install unzip
unzip chromedriver_linux64.zip
mv chromedriver /usr/bin/
```

### Additional python packages
```
pip install selenium beautifulsoup4 pandas requests
```

## Usage

You can run the notebook or modify it. Currently it only scans the first page (400 images), but this can be modified to go to the second page.