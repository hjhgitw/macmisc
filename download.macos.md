#+STARTUP: indent
* Overview
 available software

#+BEGIN_SRC sh
softwareupdate --list-full-installers
#+END_SRC



Software Update found the following full installers:
* Title: macOS Monterey, Version: 12.1, Size: 12157035487K, Build: 21C52
* Title: macOS Monterey, Version: 12.0.1, Size: 12128428704K, Build: 21A559
* Title: macOS Big Sur, Version: 11.6.2, Size: 12433351292K, Build: 20G314
* Title: macOS Big Sur, Version: 11.6.1, Size: 12428472512K, Build: 20G224
* Title: macOS Big Sur, Version: 11.6, Size: 12428553042K, Build: 20G165
* Title: macOS Big Sur, Version: 11.5.2, Size: 12440916552K, Build: 20G95
* Title: macOS Catalina, Version: 10.15.7, Size: 8248985973K, Build: 19H15
* Title: macOS Catalina, Version: 10.15.7, Size: 8248854894K, Build: 19H2
* Title: macOS Catalina, Version: 10.15.6, Size: 8248781171K, Build: 19G2021
* Title: macOS Mojave, Version: 10.14.6, Size: 6038419486K, Build: 18G103
* Title: macOS High Sierra, Version: 10.13.6, Size: 5221689433K, Build: 17G66


Download
softwareupdate --fetch-full-installer --full-installer-version 12.1
Scanning for 12.1 installer
Install finished successfully

Get Vm
https://customerconnect.vmware.com/group/vmware/evalcenter?p=fusion-player-personal&source=dwnp


sudo /Applications/Install\ macOS\ Monterey.app/Contents/Resources/createinstallmedia --volume /Volumes/USBDRIVE

Mount NTFS on MAC
hjh@MacBook-Pro ~ % mkdir ~/ntfs-volume
hjh@MacBook-Pro ~ % sudo mount -t ntfs -o rw,auto,nobrowse /dev/disk0s3 ~/ntfs-volume

https://www.paypal.com/donate/?cmd=_s-xclick&hosted_button_id=RYQ6CGUGK5D6S



Snapshots
https://derflounder.wordpress.com/2019/05/08/creating-managing-and-using-apple-file-system-snapshots-for-startup-drive-backups/

tmutil localsnapshot
NOTE: local snapshots are considered purgeable and may be removed at any time by deleted(8).
Created local snapshot with date: 2022-01-19-100832
sudo tmutil setdestination /Volumes/InMon   
hjh@C02TL0HVHTD5 ~ % sudo tmutil destinationinfo 
====================================================
Name          : InMon
Kind          : Local
Mount Point   : /Volumes/InMon
ID            : 430F47DB-7E86-4407-B6D0-2BAD26164464
hjh@C02TL0HVHTD5 ~ % 

