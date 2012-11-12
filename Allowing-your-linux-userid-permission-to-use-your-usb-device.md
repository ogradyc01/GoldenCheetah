Note: This example assumes that you know the device name of you USB device and that your userid has sudo privileges.

In this example our Linux userid is user and we are on the server called machine. Our USB device is called /dev/ttyUSB0.

Check the current permissions and owner/group of the device.

[user@machine ~]$ ls -la /dev/ttyUSB0
crw-rw----. 1 root dialout 188, 0 Apr  3 21:16 /dev/ttyUSB0 
For this configuration, the owner is root, the group is dialout and both the owner/group have read/write permissions.

What you need to do is make your login userid part of the group associated with the USB device.

For this case, we add the group dialout to our userid user using the usermod command. This command requires root privileges to run.

[user@machine ~]$ sudo usermod -a -G dialout user
You will need to log out then log back in and now you should have access to the device.