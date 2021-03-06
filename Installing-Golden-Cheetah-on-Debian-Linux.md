Debian packages are available for Golden Cheetah, directly from the Debian repositories. The Wheezy (stable) repositories contain Golden Cheetah v2.0 and the Sid (unstable)/Jessy (testing) repositories contain Golden Cheetah v3.0.

Either search for Golden Cheetah from within your package manager software, for example Synaptic, or issue the following commands from within a terminal window:

> sudo apt-get update

> sudo apt-get install goldencheetah

If you are currently running Wheezy (stable) but wish to install the latest version of Golden Cheetah, without upgrading your entire system, it is possible add the Sid repositories and then use the following commands:

> sudo apt-get update

> sudo apt-get -t unstable install goldencheetah

This will tell you of any extra dependencies needed (if any). This has potential risks and may cause problems with your entire operating system. If you don't fully understand what you are doing, avoid this step and use the version of Golden Cheetah available in the repositories for your current distribution.

If you wished to be extra cautious, some of the risk may be mitigated, and the installation can first simulated with:

> sudo apt-get  -s -t unstable install goldencheetah

Finally, disable the Sid repositories. 

This method should work with core Debian and some derivatives, for example Crunchbang. 

This process will most likely not work seamlessly with Ubuntu, unless core Debian repositories are manually added, which introduces the risks of further package conflicts.