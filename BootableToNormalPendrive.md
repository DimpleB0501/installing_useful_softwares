# In Ubuntu 18.04 
- Locate your drive `df -h`
- `sudo mkfs.vfat /dev/sdb1`
- umount it `sudo umount /dev/sdb1`

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
