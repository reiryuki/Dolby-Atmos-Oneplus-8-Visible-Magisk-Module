# Dolby Atmos OnePlus 8 Visible Magisk Module

## Descriptions
- An EQ ported from OnePlus 8 Visible (IN2015).
- It doesn't support ACDB module because using effect proxy.
- Not working with dynamic partitions (except dolby dms 2.0 is already present in ROM manifest.xml)

## Screenshots
- [OPSoundTuner](https://t.me/modsandco/6844)
- [DaxUI](https://t.me/audioryukimods/786)

## Tested on
- Redmi 4A (rolex) CRDroid Lineage based ROM Android 10 arm64-v8a

## Requirements
- Android 9, 10, or 11
- 64 bit
- Magisk installed

## Installation Guide
- Don't use ACDB module!
- Remove another Dolby module with different name
- Reboot
- If your ROM has Dolby in-built, then you need to enable Dolby data clean-up for the first time (See Optional section)
- Install via Magisk Manager or Recovery (v2.1)
- Reboot

## Optional
- If your ROM has Dolby in-built, or Dolby effects are not triggered, then you need to enable Dolby data clean-up for the first time. Run at Terminal Emulator before flashing
  the module:

  `su`

  `setprop` `dolby.force.cleanup` `1`

  After that, flash/reflash the module.

- You can rename dax-default extension to .xml to use more bass enhancer boost. See /data/adb/modules_update/DolbyAtmos/system/vendor/etc/dolby/. Rename another .xml to .mod. Delete /data/vendor/dolby/dax_sqlite3.db if there before reboot. 96 is a standard high bass.
- You can use DaxUI instead of OPSoundTuner. To enable that, run at Terminal Emulator before flashing
  the module:

  `su`

  `setprop` `dolby.force.daxui` `1`

  After that, flash/reflash the module.

- You can disable your in-built Dirac audio FX if you sure it's conflicting with Dolby. Run at Terminal Emulator before flashing
  the module:

  `su`

  `setprop` `dolby.force.disable.dirac` `1`

  After that, flash/reflash the module.

- You can disable your in-built MI Sound FX if you sure it's conflicting with Dolby. Run at Terminal Emulator before flashing
  the module:

  `su`

  `setprop` `dolby.force.disable.misoundfx` `1`

  After that, flash/reflash the module.

## Troubleshootings
- If you want to enable OPSoundTuner dark mode while activating your dark theme, go to your Developer Settings, then turn on "Override force-dark".
- If you got problem while connecting Bluetooth audio, then use DaxUI instead. See "Optional" section. Actually, OPSoundTuner is only for Bluetooth A2DP offload supported device.
- If you using Riru EdXposed or Taichi Magisk Module, exclude Dolby apps from their list to prevent SE policy patch denials.
- Install Audio Modification Library module if using multiple audio mods.
- If installation failed with "I/O error", then you need to disable DM-Verity of your ROM first.
- If installation failed with error "No space left on device", that is mean you using dynamic partitions.
- If SE policy patch doesn't work for your device, send logcats to dev, then try using force permissive method.
  Run at Terminal Emulator before flash:

  `su`

  `setprop` `dolby.force.permissive` `1`

- If Dolby force close, just reinstall again
- Make sure manifest.xml is patched correctly
- Install Audio Compatibility Patch if you encounter (deep buffer) audio processing problem. But usually no need.
- If anything goes wrong, see your logcats
  - "CANNOT LINK EXECUTABLE" mean your hardware is not supported

# Attention!
- Reporting without send full logcats and install process logs is ignored!
https://play.google.com/store/apps/details?id=com.dp.logcatapp

## Telegram
- https://t.me/audioryukimods
- https://t.me/modsandco

## Donate
- https://www.paypal.me/reiryuki



      -- Enjoy the Atmos 🎧 --


