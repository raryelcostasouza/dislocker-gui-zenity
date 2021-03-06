# zDislocker
Zenity based GUI for mounting and umounting BitLocker drives using Dislocker (https://github.com/Aorimn/dislocker)


# Recent Changes 08/04/2019

## Release v2.1 - https://github.com/raryelcostasouza/zDislocker/releases/tag/v2.1
* Rename the app to zDislocker (zenity Dislocker)
* Fix bug on installer. The line on sudoers file was being added extra times even if it was already there.

## Release v2.0 - https://github.com/raryelcostasouza/dislocker-gui-zenity/releases/tag/v2.0
* Added support for mounting/unmounting multiple BitLocker drives
* Fix bug that cause FAT partitions or disks with GPT partitioning not being detected.
* Fix bug that caused the mounted drive only to be editable by the root user

# Requirements
1. dislocker
2. zenity


# Installation instructions
sudo ./install.sh

Note: to enable non-admin users to mount/umount BitLocker protected drives, by default, during the installation a rule is added to the /etc/sudoers file. This rule allow all users to execute the script util-root.sh (where the root commands needed for mounting/umounting are located).

# WARNING!!!
The proper and safe way to eject the BitLocker encrypted drives is using this app.
Your file browser may automatically show an eject button, but it does not know how to eject with BitLocker drives properly.

If you eject a drive only using the file browser button it may cause DATA LOSS.

# Screenshots

# Main Window
![dislocker-gui-ss0](screenshot/main.png?raw=true "Main Window")

# BitLocker Drive Selection List
![dislocker-gui-ss1](screenshot/drive-list.png?raw=true "BitLocker Drive List")

# Password Input
![dislocker-gui-ss2](screenshot/password-input.png?raw=true "Password Input")

# Drive currently Mounted. Eject safely?
![dislocker-gui-ss3](screenshot/drive-mounted-eject-safely.png?raw=true "Eject Safely")

# Mount successfully
![dislocker-gui-ss4](screenshot/mount-success.png?raw=true "Mount Success")

## License

GNU GPL v3
