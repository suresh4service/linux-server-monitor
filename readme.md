#Linux Server Monitor

This is a lightweight monitoring tool for Linux servers.

https://github.com/chris-brown-nz/linux-server-monitor

It's written for Python 3.5 and has been tested with Ubuntu 16.10 64-bit. Please let me know if you have tested it on other flavours of Linux.

It monitors:

- Antivirus (last update)
- Last boot date/time and uptime (days)
- CPU usage
- Disk usage
- Load average
- Memory usage
- Internet performance
- Swap memory
- System info
- CPU temperature

#Credit

This project uses a modified version of Matt Martz's 'speedtest-cli':
* https://pypi.python.org/pypi/speedtest-cli/
* https://github.com/sivel/speedtest-cli

Matt's project is licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except in compliance with the License. You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0

#Installation

1. Modify the log_path variable at the top of the script. This is where your log file(s) will go. Example: '/home/chris/linux-server-monitor/'
2. Modify the cpu_temp dictionary at the top of the script. You can add or remove line as necessary as long as you keep the same formatting for the key.
3. Place the files somewhere in your path, e.g. '/usr/local/bin/linux-server-monitor/'
4. Make the script executable: $ chmod +x monitor.py
5. You should now be able to run the script from any directory in terminal using: $ lsm.py

Note: You should not need to run linux-server-monitor as sudo.

##Scheduling

Linux Server Monitor is not very useful unless it's scheduled to run reguarly. 

#Usage

#Contact/Support



Please log any change requests or bugs at: https://github.com/chris-brown-nz/linux-server-monitor/issues

#Changelog

Date | Version | Description
---- | ------- | -----------
2016-12-16 | --- | Initial release. Tested with Gmail API client v1.5.5, Python 3.5, Ubuntu 16.04 64-bit desktop.


# linux-server-monitor

[![Join the chat at https://gitter.im/linux-server-monitor/Lobby](https://badges.gitter.im/linux-server-monitor/Lobby.svg)](https://gitter.im/linux-server-monitor/Lobby?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

