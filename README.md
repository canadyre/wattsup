Watts Up? Python Interface
==========================

Code to interface with the Watts up? .net. Works over the USB cable. Allows you
to view samples in a terminal, save to a logfile, or POST them using the
network connection.


Usage
-----

### Linux

    python3 wattsup.py -p /dev/ttyUSBX -i
    python3 wattsup.py --help
    python3 wattsup.py -p /dev/ttyUSBX -l -f json

### Mac OS X

Install the http://www.ftdichip.com/Drivers/VCP.htm drivers. Restart.

    python wattsup.py -p /dev/tty.usbserial-X -i


### Configure POST

    ./wattsup.py -p /dev/ttyX -n myserver.com 80 /wattsup/data



Server
------

A simple python script that receives the HTTP request from Watts Up .net
and prints out the values in JSON format.
