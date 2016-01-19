All versions powertap monitor should work on GoldenCheetah.</br>
On ubuntu GoldenCheetach should be compiled with D2XX driver  http://www.ftdichip.com/Drivers/D2XX.htm 

entry D2XX_INCLUDE in  src/gcconfig.pri

    # If you want D2XX device downloads, you need the D2XX libraries    
    #    http://www.ftdichip.com/Drivers/D2XX.htm    
    # Set path to where the D2XX include file (d2xx.h) is located    
    # If the files are in /usr/include/d2xx then set    
    D2XX = /home/witold/Pobrane/d2xx/release     
    # If for some reason you need a library to compile d2xx support
    # specify it on the D2XX_LIBS = line.
    # You *must* define D2XX_INCLUDE to use this feature.
    D2XX_INCLUDE =  /usr/include  
    D2XX_LIBS    =  /usr/local/lib/libftd2xx.so

and recomile GC



Special usb device should have own udev rule

    witold@dom:~$ lsusb      
    Bus 004 Device 002: ID 8087:0024 Intel Corp. Integrated Rate Matching Hub 
    Bus 004 Device 001: ID 1d6b:0002 Linux Foundation 2.0 root hub
    Bus 002 Device 001: ID 1d6b:0003 Linux Foundation 3.0 root hub
    Bus 001 Device 003: ID 413c:3016 Dell Computer Corp. Optical 5-Button Wheel Mouse
    Bus 001 Device 002: ID 413c:2003 Dell Computer Corp. Keyboard
    Bus 001 Device 001: ID 1d6b:0002 Linux Foundation 2.0 root hub
    Bus 003 Device 005: ID 0403:6001 Future Technology Devices International, Ltd FT232 USB-Serial (UART) IC
    Bus 003 Device 002: ID 8087:0024 Intel Corp. Integrated Rate Matching Hub
    Bus 003 Device 001: ID 1d6b:0002 Linux Foundation 2.0 root hub

next create

    witold@dom:$ sudo touch /etc/udev/rules.d/11-joulegps.
    witold@dom:$ cat /etc/udev/rules.d/11-joulegps. 
    SUBSYSTEMS=="usb", ATTRS{idVendor}=="0403", ATTRS{idProduct}=="6001", GROUP="dialout", MODE="0666"

idVendor and idProduct are from lsusb  after ID -> 0403:6001...  

and restart udev for change

    witold@dom:~$ sudo /etc/init.d/udev restart    


unload ftdi_sio and usbserial and restart GC

    witold@dom:~$ sudo rmmod ftdi_sio    
    witold@dom:~$ sudo rmmod usbserial    


Tested on ubuntu 14.04 LTS