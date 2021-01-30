# In Ubuntu 
Unmount all currently mounted partitions on that device, if any. Then run the following, replacing /dev/sdX with the name of your device:

sudo shred -v /dev/sdX

This will overwrite all the blocks on the device with random data three times, the -v flag is for verbose and will print the current progress.

You can add the option -nN to only do this N times, to save time on large capacity devices. This might take a while, depending on the size of your external hard drive (I think it takes twenty minutes or so for my 4 GB flash drive).

You can also set all bits to zero after the last iteration by adding the option -z, I prefer to do this.

sudo shred -v -n1 -z /dev/sdX

After this, you would have to repartition the device. The easiest way is to install GParted and use it:

sudo apt-get install gparted
gksu gparted

Choose your device in the upper-right corner list. Then select Device -> Create partition table to create a partition table on the device.

Then add a single partition that uses all of the unallocated space on the device, choosing fat32 as the file system. Apply the changes by click the Apply button (the green checkmark) in the toolbar.

# In Windows
- Run `cmd` as Administrator <br/>
- Type `DISKPART`<br/>
- `list disk`<br/>
- `select disk 1` (if your usb drive mine was 1)<br/>
- `clean`<br/>
- `create partition primary`<br/>
- `active`<br/>
- Choose a format:<br/>
  - FAT32 is the standard for USBs: `format fs=fat32 quick`<br/>
  - NTFS is more modern, but isn't as widely supported it is compatible with Windows: `format fs=ntfs quick`<br/>
- `assign`<br/>
- `exit`<br/>
- `exit`<br/>
