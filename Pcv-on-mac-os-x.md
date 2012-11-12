# PCV on Mac OS X

We're generally recommending the drivers from this site:

http://osx-pl2303.sourceforge.net/

For Mac OS X Lion (10.7) in 64bit mode, the following build is known to work:

http://changux.co/osx-installer-to-pl2303-serial-usb-on-osx-lio

which is based on the changes from here:

http://xbsd.nl/2011/07/pl2303-serial-usb-on-osx-lion.html

Successfull instalation of these drivers can be verified (with the cable plugged in) with the following terminal command:

ls -l /dev/cu.PL2303-*

We recommend running Golden Cheetah v2.1 or v3.x as there enhancements in the code when talking to PCV.