# Install

### Create bootable USB drive from OSX

```
hdiutil convert /path/to/ubuntu.iso -format UDRW -o /path/to/target.img
diskutil list
diskutil unmountDisk /dev/diskN
sudo dd if=/path/to/downloaded.img of=/dev/diskN bs=1m
diskutil eject /dev/diskN
```
