The realtime racing mode (available from the training and racing view) requires you to configure the devices you wish to use. For v2.0 and greater, currently, three kinds of devices are supported; Computrainer (via Serial or Serial-to-USB adapter) Golden Cheetah Server or ANT+ via Quarq's Quarqd. From v3.0 onwards Golden Cheetah supports Native ANT+.

_Device support has been in active development and this information is up to date for dev builds as of mid November 2012._

From the configuration dialog box (Tools->Options or Golden Cheetah->preferences on a Mac) you should select the Devices icon at the bottom on the left. From here you will be able to add or delete devices to the device list shown in the table. Each device is given a name and type. Use the name to distinguish between devices that you have. Once the device is setup, you need to select it in the 'Workout Library' and click the play button in the the 'Train' tab. Data from your device should display in the boxes at the top of screen.

At the moment, only a single device source (ie. Either Native ANT+ or Computrainer, not both) can be active at one time.

Instructions for setting up device types:

## Native ANT+ (Version 3.0+)
For a Native ANT+ device you will need a USB stick such as:

http://www.sparkfun.com/products/8840
https://buy.garmin.com/shop/shop.do?pID=10997

You can often find the Garmin sticks on EBay:
http://www.ebay.com/sch/i.html?_nkw=garmin+010-10999-00

### A note for all Operating System - Pairing with ANT+
Please note that under ANT+ there is at this time no concept of Pairing. If you hit the Pair button it will fail.

Please just start your training session in GoldenCheetah and start pedaling.
GoldenCheetah will find your devices and display the data.

### Running on Mac OSX
For the Garmin USB1 stick you will need to install device drivers:

http://www.silabs.com/products/mcu/Pages/USBtoUARTBridgeVCPDrivers.aspx or
http://www.thisisant.com/images/Resources/20090717-Silicon%20Labs%20USB%20Driver%20Installer.mpkg.zip

Once the drivers are installed and the computer has been restarted, you can plug in your USB stick and you should get a device file called /dev/cu.ANTUSBStick.slabvcp. This is the device port that you should enter when creating the device in GoldenCheetah.

For the Garmin USB2 stick, newer versions of OSX should find the stick.
To check this is the case, start Terminal, run the following command and then insert the USB stick:

`tail -f /var/log/system.log`

You should see the device being inserted and recognized. Add the Device to Golden Cheetah and set the Device Profile to: /dev/ignored as it is not actually needed for anything but getting around the checks in the dialog box. This should hopefully be fixed in the future.

### Running on Windows
For the Garmin USB1 stick you will most likely need to download and install device drivers:
http://www.thisisant.com/images/Resources/1208970787_ANT%20USB%20Drivers.zip

For the Garmin USB2 stick Windows should identify the device and install the driver. If not you can use:
http://www.thisisant.com/images/Resources/ant%20usb2%20drivers.zip

Once the drivers are installed you can create your device in GoldenCheetah. No Device Profile is needed.

### Linux

With the latest builds of GCv3 there is very little set up required.
You need to give your ANT+ stick read write permissions.
To do this, create a file:
`/etc/udev/rules.d/51-garmin-usb.rules`
containing the following line:
`ATTRS{idVendor}=="0fcf", ATTRS{idProduct}=="1008", MODE="0666"` 
In the command line you could do this (as root):
`echo 'ATTRS{idVendor}=="0fcf", ATTRS{idProduct}=="1008", MODE="0666"' >> /etc/udev/rules.d/51-garmin-usb.rules`
Then in GC:

* A sensible device name should be chosen.
* Device Port needs to be populated, but is not used – just add something like '/dev/ttyANT'.
* To set up a workout, simply select your new device, press 'start', and begin pedaling. It should just work.
**Older versions with Linux**
For the Garmin USB1 stick you will generally need to have libusb installed. GoldenCheetah is known to work with libusb 0.1.12. Other versions may or may not work. Install the library and then restart your machine. Insert the USB stick. Take a look in /dev/ and it will normally be ttyUSBx where x is a number starting at 0. This is the device to put into your Device Port (eg. /dev/ttyUSB0)

For the Garmin USB2 stick, things can be a little tricker. Hopefully the device should be found and appear in /dev/ as per the USB1 stick. If not, check out the following from Mark Rages who knows a thing or two:

It has been reported for Ubuntu that running the following command: 

 sudo modprobe usbserial vendor=0x0fcf product=0x1008

will make the Ant+ stick show up as ttyUSB0.
To make the change permanent, you can do 

echo "options usbserial vendor=0x0fcf product=0x1008" > /etc/modprobe.d/ant-usb2.conf

(do it as root, sudo s makes you root) 
If, like me, you have a bunch of different USB>serial devices, you might want to give the stick a consistent filename: 
echo 'SUBSYSTEM=="tty" ACTION=="add" ATTRS{idProduct}=="1008" ATTRS{idVendor}=="0fcf" SYMLINK+="ttyANT"' \
> /etc/udev/rules.d/10-antstick.rules

(do it as root, all on a line). 
Then use "/dev/ttyANT" as the Device Profile.
Computrainer
The device port is the communication port the computrainer is attached to, under windows this will be a com port (COM0 - COM32) whilst under Linux and Mac this is the /dev device file related to the Serial/USB adapter you are using. For example, the Keyspan USB adapter is often available from "/dev/cu.KeySerial1".

To identify the device in question it is simplest to plug the USB adaptor in, connect your computrainer and then list the device files with "ls -lt /dev/cu.*" in a terminal window. Often the device file can be seen by running "dmesg" in the terminal window.

ctAnt+ (http://www.ct-ant.com/)
From this thread: http://groups.google.com/group/golden-cheetah-users/browse_thread/thread/4a10d3d3ed1b565f

I've got ctANT+ working with GC3 on my WinXP system. The key thing, for me anyway, is launch order. This is what works for me:
Launch ctANT+
Activate ctANT+ and wait for your various devices to pair and show as Paired. At this point, the Computrainer should show as "Unit Connected" and "Awaiting Data".
Launch GC3, navigate to the Train page and select your Computrainer and .erg file.
Hit "Play". At that point, the CT status in ctANT+ should change from "Awaiting Data" to "Feeding Data".
The critical part is having ctANT+ running and active before launching GC3.

Golden Cheetah Server
I have no idea what this is.

ANT+ via Quarqd (Version 2.x+)
Native ANT+ is now the preferred method for connecting a ANT+ device in versions 3.0 and above.
For realtime setup of ANT+ devices in version 2.x, here are older instructions for setting up via Quarqd.

quarqd setup (Windows)
quarqd setup (Linux/Mac)