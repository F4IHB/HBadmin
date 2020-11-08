# HBadmin
Admin panel for **HBlink** servers

This tool will be develop in Python (version 3) same like HBlink and HBmonitor.

## Features
HBadmin is a Graphical User Interface for editing **HBlink** config file.

You will be able to :
- Edit general settings  : Global, Logging, Aliases & Reports
- Edit instances : Masters, Peers, OpenBridges and XLX Peers
- Backups and restore the **HBlink** config file
- Monitor (very light) your server : CPU & RAM usage, disk space

![Preview of HBadmin](http://f4ihb.fr/data/medias/hbadmin-preview1.png "Preview of HBadmin")


## Installation guide

November 8, 2020 : It's just a reminder.

```bash
cd /opt
git clone https://github.com/F4IHB/HBadmin.git 

cd HBadmin

cp config_SAMPLE.py config.py
nano config.py

cp /opt/HBadmin/hbadmin.service /lib/systemd/system/hbadmin.service

systemctl enable hbadmin.service
systemctl start hbadmin.service
```
