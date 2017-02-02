#Linux Server Monitor

This is a lightweight monitoring tool for Linux servers.

https://github.com/chris-brown-nz/linux-server-monitor

It's written for Python 3.5 and has been tested with Ubuntu 16.10 64-bit desktop. I will shortly be rolling it out to my Ubuntu 16.10 servers. Please let me know if you have tested it on other flavours/versions of Linux.

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

1. Modify the log_dir variable at the top of the script. This is where your log file(s) will go. Example: '/home/chris/linux-server-monitor/'
2. Modify the cpu_temp dictionary at the top of the script. You can add or remove line as necessary as long as you keep the same formatting for the key.
3. Place the files 'lsm' and 'lsm_speedtest.py' somewhere in your path, e.g. '/usr/local/bin/'
4. Make the script executable: $ chmod +x monitor.py

Note: You should not need to run linux-server-monitor as sudo.

#Usage

You can use Linux Server Monitor from anywhere: $ lsm

##Scheduling

Linux Server Monitor is most useful when scheduled to run regularly.
 
1. Go to your crontab editor: $ crontab -e
2. Add a line to run at a scheduled interval, e.g. 2 minutes: */2 * * * * /usr/local/bin/lsm
 

#Contact/Support

You can contact me with general comments and enquiries via: https://gitter.im/linux-server-monitor/linux-server-monitor

Please log any change requests or bugs at: https://github.com/chris-brown-nz/linux-server-monitor/issues

#Changelog

Date | Version | Description
---- | ------- | -----------
2017-02-02 | 0.0.1 | Initial release. Tested with Python 3.5, Ubuntu 16.04 64-bit desktop.






