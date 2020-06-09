# CUHK-Internet-Autologin


## Requirements
Python3 is suggested, but through minor editing this code can be ran on python2.

Install the dependencies from pip.
```
pip install -r requirements.txt
```

For Raspberry Pi, a chromedriver designed for corresponding ARM architecture is needed. <br>
In Raspbian Buster, replace the chromedriver binary with:
```
sudo apt install chromium-chromedriver
rm -f ./chromedriver
ln -s $(realpath /usr/lib/chromium-browser/chromedriver)
```

## How To Use
Run the following command to start auto monitoring.
```
python monitor.py
```

You may also run the following command to test if the log-in function works.
```
python login.py
```

## Settings
Edit your username and password inside `login.py`

Period for checking internet connection can be adjusted inside `monitor.py` at `SLEEP_TIME`, in terms of seconds. 

