# ASUS-C434TA-DSM4T-Opencore-EFI

WIP Opencore EFI for ASUS Chromebook Flip C434TA-DSM4T running MacOS Sonoma (14). For the most part, it boots and can function but some features are lacking. Still need to apply Chromebook-specific patches and fixes. Currently using a custom version of Coreboot; many issues are patched through this [version](https://github.com/Chromeintosh/coreboot).

## To Do

- [x] Boots?
- [x] Map USB Ports
- [x] Fix Touchpad
- Double check the following for ACPI:
  - [x] SSDT-PLUG-ALT.aml
  - [x] Top row keyboard remap SSDT
  - [x] Fake ambient light sensor SSDT
  - [x] FixHPET SSDT generated
- Double check the following for Kexts:
  - [x] eMMC Driver
  - [x] Replace Default VoodooPS2 Kext
  - [x] EC Kext for functional EC/Keyboard backlight
- Config.plist patches:
  - [x] Set SMBIOS
  - [x] ProtectMemoryRegions
  - [x] PciRoot(0x0)/Pci(0x2,0x0) 
- [x] VoodooI2CHID.kext for touchscreen (due to having a C434T)
- [x] Merge HPET patches (in ACPI for ACPI->Patches) 

# Post-Install Tasks

- [ ] Fix Audio
- [ ] Fix sleep/power issues
- [ ] WiFi-related issues with itlwm

Source: <https://docs.meghan6.com/docs/installingmacos/installing>

Thank you @meghan6 and @ethanaobrien for the help! I am NOT affiliated with Chrultrabook and/or Chromeintosh in any way, shape, or form. Please do not contact them for support.
