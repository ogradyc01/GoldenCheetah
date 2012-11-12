## Version 2.1.0 and earlier version

* Install the GoldenCheetah to your USB drive, thumb drive, whatever.
* Right next to the GoldenCheetah executable on the USB Drive, create a folder called "Library" and inside that folder create another folder called "GoldenCheetah".
* Launch GC from the USB drive, create your cyclist from inside GC.
* Take the rider data and copy it to Library/GoldenCheetah/<CYCLISTNAME> (on the USB drive)
* Restart GC, the rides should be there

## Development Version 3.0.0

* Install the GoldenCheetah to your USB drive, thumb drive, whatever.
* Right next to the GoldenCheetah executable on the USB Drive, create a folder called "Library" and inside that folder create another folder called "GoldenCheetah-v3".
* Launch GC from the USB drive, create your cyclist from inside GC.
* Take the rider data and copy it to `Library/GoldenCheetah-v3`/<CYCLISTNAME>` (on the USB drive)
* Restart GC, the rides should be there

Basically, GC first looks to see if `Library/GoldenCheetah` [or `Library/GoldenCheetah-v3` for 3.0 development versions] exists next to where the executable is. If it finds those series of folders, it loads the data from there. If not, it loads the data based on the OS.

You can also keep Mac, Linux and Windows versions of the executable on the drive so you have a multi-platform solution.