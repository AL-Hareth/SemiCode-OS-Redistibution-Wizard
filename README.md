SemiCode OS Redistibution Wizard
=========================

This project is brought to you by semicode.org ,  SemiCode OS is 
a new Linuk Distro for Programmers & Developers.  
Too often do users need to customize open source operating systems, 
such as SemiCode OS, to work correctly on their machines.  By distributing 
a custom SemiCode OS distro with the kinks worked out for your machine, you 
would be helping others to run SemiCode OS if they have the same machine.



SemiCode OS Redistibution Wizard creates an installable Live ISO from an installed 
SemiCode OS or derivative distribution.

It is a bash script, similar to Remastersys and its forks.  The script is 
based on this tutorial: https://help.ubuntu.com/community/MakeALiveCD/DVD/BootableFlashFromHarddiskInstall. 

To run the script, run it from the directory where it is located.  For example:


cd ~/distroshare-ubuntu-imager-1.0
./distroshare-ubuntu-imager.sh

To boot the ISO from a USB stick, you can use the dd command like this:

dd if=isoimage.iso of=/dev/sdb bs=1M

where sdb is your USB drive.  You should be able something similar on Mac OS X.
You can also use UNetbootin: http://unetbootin.sourceforge.net/ to create a 
bootable USB drive.

Ubuntu Startup Disk creator won't be able to turn the iso into a bootable 
usb drive since Distroshare Ubuntu Imager uses grub2 as the bootloader.
