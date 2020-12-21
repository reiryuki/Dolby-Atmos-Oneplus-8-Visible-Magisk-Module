# Dolby Atmos OnePlus 8 Visible Magisk Module

## Descriptions
- An EQ ported from OnePlus 8 Visible (IN2015).
- It doesn't support ACDB module because using effect proxy.
- Not working with dynamic partitions.

## Tested on
- Redmi 4A (rolex) CRDroid Lineage based ROM Android 10 arm64-v8a

## Requirements
- Android 9, 10, or 11
- 64 bit
- Magisk installed

## Installation Guide
- Don't use ACDB module!
- Remove another Dolby module
- Reboot
- Install via Magisk Manager only
- Reboot

## Optional
- You can rename dax-default extension to .xml to use more bass enhancer boost. See /data/adb/modules_update/DolbyAtmos/system/vendor/etc/dolby/. Rename another .xml to .mod. Delete /data/vendor/dolby/dax_sqlite3.db if there before reboot.
- You can use DaxUI instead of OPSoundTuner. To enable that, run at Terminal Emulator before flashing
  the module:

  `su`

  `setprop dolby.force.daxui 1`

  After that, flash (reflash) the module.

## Troubleshooting
- If you got problem while connecting Bluetooth audio, then use DaxUI instead. See "Optional" section.
- Install Audio Modification Library module if using multiple audio mods.
- If installation failed with "I/O error", then you need to disable DM-Verity of your ROM first.
- If installation failed with error "No space left on device", that is mean you using dynamic partitions.
- If SE policy patch doesn't work for your device, send logcats to dev, then try using force permissive method.
  Run at Terminal Emulator before flash:

  `su`

  `setprop dolby.force.permissive 1`

- If Dolby force close, just reinstall again
- Make sure manifest.xml is patched correctly
- Install Audio Compatibility Patch if you encounter (deep buffer) audio processing problem.

# Attention!
- Reporting without send full logcats and install process logs is ignored!
https://play.google.com/store/apps/details?id=com.dp.logcatapp

## Telegram
- https://t.me/audioryukimods
- https://t.me/modsandco

## Donate
- https://www.paypal.me/reiryuki



          -- Enjoy the Atmos 🎧 --


