# FWFlash3
Bash script to write a disk image to a (theoretically) unlimited number of USB flash drives or other media / bulk replication. This script is designed to only target drives that are the same size as the one specified in the launch command which means it works best when all flash drives were sourced by the same manufacturer - be sure to unplug all flashdrives you want to exclude while running this script

###USE AT OWN RISK##
Comment out lines 20 and 23 to do a dry run

Directions to run
1) Clone the repisitory
2) chmod +x FWFlash3
3) Launch a terminal and run the following

sudo ./FWFlash3 -s "7.5G" -i /path/to/image.img

-s is the size of the storage devices you want to target (use "lsblk" to find the sizes)
-i is the path to the image file (this can be any disk image that can be written to a flash drive including img files, iso files, ChromiumOS .bin images, and more)

