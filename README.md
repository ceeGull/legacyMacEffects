# legacyMacEffects
Makes the menubar and windows have effects for example the menu and menubar has dropshadows when clicking on the apple menu an inner shadow is seen
On anything in the window header there is a dropshadow (note not implemented for dark mode)

# Installation
Please note before installation if your running macOS BigSur or greater that you need to follow this [guide](https://github.com/jslegendre/ThemeEngine) otherwise this will not work
If your running anything before BigSur than you can skip this part

ALSO BACKUP `/System/Library/CoreServices/SystemAppearance.bundle` BEFORE DOING THIS!!

1. Boot into Recovery-mode and disable SIP (System Integrity Protection) by using the terminal and type
   `csrutil disable`

2. Once done reboot, open the terminal and type
   `sudo defaults write /Library/Preferences/com.apple.security.libraryvalidation.plist DisableLibraryValidation -bool true` <-- this will disable library validation

3. Reboot and finally onto the terminal and type
   `sudo mount -uw /` <-- unlocks the system for modification

4. Copy `VibrantLightApperance.car` and Go to `/System/Library/CoreServices/SystemAppearance.bundle` and right click `Show Package Contents` and Go to `Contents/Resources`
   Paste `VibrantLightAppearance.car`
   - Alternatively type into the terminal `sudo cp VibrantLightAppearance.car /System/Library/CoreServices/SystemAppearance.bundle/Contents/Resources/` <-- Copies the modded file to the respective file

5. The theme should be applied either by opening an App or logging out and logging back in
