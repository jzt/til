# os

## Ubuntu

### Create Ubuntu bootable USB from macOS
```
hdiutil convert -format UDRW -o ubuntu-16.04.2-desktop-amd64.img ubuntu-16.04.2-desktop-amd64.iso
mv ubuntu-16.04.2-desktop-amd64.img.dmg ubuntu-16.04.2-desktop-amd64.img
diskutil list
diskutil unmountDisk /dev/disk3
sudo dd if=ubuntu-16.04.2-desktop-amd64.img of=/dev/rdisk3 bs=1m
diskutil eject /dev/disk3
```
