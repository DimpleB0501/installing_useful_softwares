# In Ubuntu 18.04 
- Locate your drive `df -h`
- `sudo mkfs.vfat /dev/sdb1`
- umount it `sudo umount /dev/sdb1`

# In Windows
Run `cmd` as Administrator
Type `DISKPART`
`list disk`
`select disk 1` (if your usb drive mine was 1)
`clean`
`create partition primary`
`active`
Choose a format:
 - FAT32 is the standard for USBs: `format fs=fat32 quick`
 - NTFS is more modern, but isn't as widely supported: `format fs=ntfs quick`
`assign`
`exit`
`exit`
