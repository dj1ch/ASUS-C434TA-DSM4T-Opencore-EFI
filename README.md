# ASUS-C434TA-DSM4T-Opencore-EFI

WIP Opencore EFI for ASUS Chromebook Flip C434TA-DSM4T running MacOS Sonoma (14). For the most part, it boots and can function but some features are lacking. Still need to apply Chromebook-specific patches and fixes. Currently using a custom version of Coreboot; many issues are patched through this [version](https://github.com/Chromeintosh/coreboot).

## To Do

- [x] Boots?
- [] Map USB Ports?
- [] Fix Audio
- [] Fix Touchpad
- Double check the following for ACPI:
  - [] SSDT-PLUG-ALT.aml
  - [] Top row keyboard remap SSDT
  - [] Fake ambient light sensor SSDT
  - [] FixHPET SSDT generated
- Double check the following for Kexts:
  - [] eMMC Driver
  - [] Replace Default VoodooPS2 Kext
  - [] EC Kext for functional EC/Keyboard backlight
- Config.plist patches:
  - [] Set SMBIOS
  - [] ProtectMemoryRegions
  - [] PciRoot(0x0)/Pci(0x2,0x0) 
- [] VoodooI2CHID.kext for touchscreen (due to having a C434T)

Source: <https://docs.meghan6.com/docs/installingmacos/installing>

Thank you @meghan6 and @ethanaobrien for the help! I am NOT affiliated with Chrultrabook and/or Chromeintosh in any way, shape, or form. Please do not contact them for support.
