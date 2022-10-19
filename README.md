# RouterSploit - Exploitation Framework for Embedded Devices

[![Python 3.6](https://img.shields.io/badge/Python-3.6-yellow.svg)](http://www.python.org/download/)
[![Build Status](https://travis-ci.org/threat9/routersploit.svg?branch=master)](https://travis-ci.org/threat9/routersploit)

The RouterSploit Framework is an open-source exploitation framework dedicated to embedded devices.

[![asciicast](https://asciinema.org/a/180370.png)](https://asciinema.org/a/180370)

It consists of various modules that aid penetration testing operations:

* exploits - modules that take advantage of identified vulnerabilities
* creds - modules designed to test credentials against network services
* scanners - modules that check if a target is vulnerable to any exploit
* payloads - modules that are responsible for generating payloads for various architectures and injection points
* generic - modules that perform generic attacks 

# Installation

## Requirements

Required:
* future
* requests
* paramiko
* pysnmp
* pycrypto

Optional:
* bluepy - Bluetooth low energy 

## Installation on Kali Linux

```
apt-get install python3-pip
git clone https://github.com/inj3ction/routersploit
cd routersploit
python3 -m pip install -r requirements.txt
python3 rsf.py
```

Bluetooth Low Energy support:
```
apt-get install libglib2.0-dev
python3 -m pip install bluepy
python3 rsf.py
```

## Installation on Ubuntu 20.04

```
sudo apt-get install git python3-pip
git clone https://github.com/inj3ction/routersploit
cd routersploit
python3 -m pip install -r requirements.txt
python3 rsf.py
```

Bluetooth Low Energy support:

```
sudo apt-get install libglib2.0-dev
python3 -m pip install bluepy
python3 rsf.py
```

## Installation on Ubuntu 18.04 & 17.10

```
sudo add-apt-repository universe
sudo apt-get install git python3-pip
git clone https://github.com/inj3ction/routersploit
cd routersploit
python3 -m pip install setuptools
python3 -m pip install -r requirements.txt
python3 rsf.py
```

Bluetooth Low Energy support:
```
apt-get install libglib2.0-dev
python3 -m pip install bluepy
python3 rsf.py
```


## Installation on OSX

```
git clone https://github.com/inj3ction/routersploit
cd routersploit
sudo python3 -m pip install -r requirements.txt
python3 rsf.py
```

## Running on Docker

```
git clone https://github.com/inj3ction/routersploit
cd routersploit
docker build -t routersploit .
docker run -it --rm routersploit
```

# Update

Update RouterSploit Framework often. The project is under heavy development and new modules are shipped almost every day.

```
cd routersploit
git pull
```
