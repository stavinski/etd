# Evil Twin Detector

Monitor for Evil Twin access points and be alerted of their presence

## Approach

The monitor will put the WLAN device specified into monitor mode and will scan for beacon frames being broadcast, at the same
it will periodically hop channels, it then compares the bssid & ssid against a configured whitelist and any found that do not
match will then be recorded and an alert sent.

## Install

```
pip install -r requirements.txt
git clone https://github.com/stavinski/etd.git && cd etd
```

## Usage

_change settings in etd.conf or use separate config file_

```
etd.py [-h] [-v] [-c CONFIG]

EvilTwin Detector tool - Mike Cromwell 2018

optional arguments:
  -h, --help            show this help message and exit
  -v, --verbose         add extra logging
  -c CONFIG, --config CONFIG
                        use different config file
```
