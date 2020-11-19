# Dolby Atmos OnePlus 8 Visible Magisk Module

## Descriptions
- An EQ ported from OnePlus 8 Visible (IN2015).
- It's still using UI from another for now.
- It doesn't support ACDB because using effect proxy.
- Not working with dynamic partitions.

## Tested on
- Redmi 4A (rolex) CRDroid Lineage based ROM Android 10 arm64-v8a

## Requirements
- Android 9, 10, or 11
- 64 bit
- Magisk installed
- Pass this [Signature Test App](https://t.me/audioryukimods/24)
- If doesn't pass, by using APKTool PC, resign daxService.apk using your device framework platform keys.

## Installation Guide
- Don't use ACDB!
- Remove another Dolby module
- Reboot
- Install via Magisk Manager only
- Reboot

## Optional
- If using multiple audio mods, use Audio Modification Library module.
- You can rename dax-default extension to use more bass enhancer boost. See /data/adb/modules_update/DolbyAtmos/system/vendor/etc/dolby/

## Troubleshooting
- If SE policy patch doesn't work for your device, send logcats to dev, then try using force permissive method.
  Run at Terminal Emulator before flash:
  - `su`
  - `setprop dolby.force.permissive 1`
- If Dolby force close, just reinstall again
- Make sure manifest.xml is patched correctly
- Use Audio Compatibility Patch if you encounter processing problem.

# Attention!
- Reporting without send full logcats and install process logs is ignored!
https://play.google.com/store/apps/details?id=com.dp.logcatapp
- Tap "Releases" bellow
