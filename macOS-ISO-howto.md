## Download
First download the install app bundle. Older versions can be hard to find but the current version of the time you read this, can be found in the App Store.

## Create and attach a drive wtih hdiutil
To create a drive run this command: `hdiutil create -o /tmp/Monterey.cdr -size 17000m -layout SPUD -fs HFS+J`.  
Next you will need to mount that drive `
`.  

## Create installation media in the new drive
Use the downloaded app bundle to create the media: `sudo /Applications/Install\ macOS\ Monterey.app/Contents/Resources/createinstallmedia --volume /Volumes/install_build`.  

## Convert to ISO
Move the drive to your desktop: `mv /tmp/Monterey.cdr.dmg ~/Desktop/InstallSystem.dmg`.  
Detach the drive: `hdiutil detach /Volumes/Install\ macOS\ Monterey`.  
Covnert it: `hdiutil convert ~/Desktop/InstallSystem.dmg -format UDTO -o ~/Desktop/Monterey.12.1.iso`.  

## Change file extension
The resulting file will be `~/Desktop/Monterey.12.1.iso.cdr`. Rename this file to `~/Desktop/Mojave.iso` and choose "use .iso" from the dialog. And you're all set!
