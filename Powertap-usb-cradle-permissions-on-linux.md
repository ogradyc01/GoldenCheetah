You may experience "Permission denied" error messages on Linux when trying to access the USB device. This is because, under Linux, USB devices tend to have restricted access by default.

To rectify this you, on most distributions of Linux, the 'udev' daemon will monitor USB devices and adjust the permissions according to rules the user can define. So we need to create a udev rules file to ensure that when a Powertap USB cradle is plugged in the device is adjusted to have permissions that will allow normal users (not superusers) to access the device file.

To do this:

Create a file "_/etc/udev/rules/powertap.rules_" containing the following line:

`SYSFS{idVendor}=="0403", SYSFS{idProduct}=="6001", MODE="666", GROUP="plugdev"`

(Many thanks to Gary Smith for providing this information.)