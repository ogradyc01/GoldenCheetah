Note: This example assumes that you know the device name of you USB device and that your userid has sudo privileges.

In this example our Linux userid is _user_ and we are on the server called _machine_.

Our USB device is called _/dev/ttyUSB0_.

Check the current permissions and owner/group of the device.

`[user@machine ~]$ ls -la /dev/ttyUSB0

crw-rw----. 1 root dialout 188, 0 Apr  3 21:16 /dev/ttyUSB0`
 
For this configuration, the owner is _root_, the group is _dialout_and both the owner/group have _read/write_ permissions.

What you need to do is make your login userid part of the group associated with the USB device.

For this case, we add the group _dialout_ to our userid _user_ using the _usermod_ command. This command requires root privileges to run.

`[user@machine ~]$ sudo usermod -a -G dialout user`

You will need to log out then log back in and now you should have access to the device.