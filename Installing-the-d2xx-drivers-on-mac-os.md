# Installing the D2XX Drivers on Mac OS

We've created an installer to automate the process listed below. You can download the installer here:
http://bugs.goldencheetah.org/attachments/download/248/Install_D2XX_drivers.mpkg.zip

Expand the .zip archive and double click the .mpkg file to install.

If you want to do it the old fasioned way, follow the steps below.

This will guide you through the steps to install the D2XX drivers required for downloading form a powertap into GoldenCheetah.

You may find it easiest to copy and paste the commands for each step to the terminal to avoid typos.

# Download the drivers from here: http://bugs.goldencheetah.org/attachments/download/1/Universal_D2XX0.1.6.dmg
# mount the disk image by double clicking the .dmg file
# drag the D2XX folder to the Desktop
# Open a Terminal window (Finder->Go->Utilities->Terminal).
# Create the /usr/local/lib directory by typing the following line in terminal followed by a return:
@sudo mkdir -p /usr/local/lib@
# Copy the dylib file to /usr/local/lib 
@sudo cp Desktop/D2XX/bin/libftd2xx.0.1.6.dylib /usr/local/lib/libftd2xx.0.1.6.dylib@
# Make a symbolic link :
@sudo ln -sf /usr/local/lib/libftd2xx.0.1.6.dylib /usr/local/lib/libftd2xx.dylib@
# You have now successfully installed the D2XX drivers. 
