# Tweaks for Linux on the CHUWI Minibook X

This is a collection of tweaks I have found in various repos and forums, for Linux on the Minibook X N150.
I am running CachyOS (Arch Linux) and KDE Plasma, but this should be applicable on any distro.

## Github repos
- https://github.com/rhalkyard/minibook-dual-accelerometer
- https://github.com/greymouser/minibook-x-tools
- https://github.com/sonnyp/linux-minibook-x

## Fix display low refresh rate
https://github.com/sonnyp/linux-minibook-x/issues/7

## Touchpad jitter

## BIOS Unlock
https://raw.githubusercontent.com/greymouser/minibook-x-tools/refs/heads/main/tools/n150-ec-byte-bios

### My BIOS settings
* Chipset -> PCH-IO Configuration
	* eMMC -> SCS Configuration **disabled**
	* SATA Configuration -> **Disabled** 
* Advaned ->Power & Perforance -> CPU ->  CPU Lock configuration -> **Disable** (doesn't seem to make a difference)
* Chipset - PCH-IO Configuration - PCI Express Configuration - DMI Link ASPM Control - L0sL1 (Seemed to enable lower c-states)

### Unlock higher C-States
