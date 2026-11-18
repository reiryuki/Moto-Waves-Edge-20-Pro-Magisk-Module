# Moto Waves V2 Edge 20 Pro Magisk Module

## DISCLAIMER
- Motorola and Waves apps and blobs are owned by Motorola™ and Waves™.
- The MIT license specified here is for the Magisk Module only, not for Motorola and Waves apps and blobs.

## Description
Equalizer global type sound effect ported from Motorola Edge 20 Pro (pstar) and integrated as a Magisk Module for all supported and rooted devices with Magisk

## Sources
- https://dumps.tadiphone.dev/dumps/motorola/pstar user-13-T1RAA33.39-11-2-ef936f-release-keys
- MotoWavesV2.apk new UI by @Bobbyishere7
- system_support: LineageOS ROM Android 14
- libmagiskpolicy.so: Magisk (debug) 31.0 (31000)

## Screenshots
- Original UI: https://t.me/androidryukimods/1063
- New UI: https://t.me/ryukimodsscreenshots/168

## Requirements
- armeabi-v7a or arm64-v8a with armeabi-v7a support architecture
- 32 bit HIDL audio service
- Android 11 (SDK 30) and up
- Magisk or Kitsune Mask or KernelSU or Apatch installed
- For original UI variant, Moto Core Magisk Module is required https://github.com/reiryuki/Moto-Core-Magisk-Module except you are in Motorola ROM
- For new UI variant, Moto Core Magisk Module is not required
- Bluetooth A2DP offload ROM support for Bluetooth audio

## Download Links and Changelog

v1.7 Original UI https://github.com/reiryuki/Moto-Waves-Edge-20-Pro-Magisk-Module

v1.7 New UI https://github.com/reiryuki/Moto-Waves-Edge-20-Pro-Magisk-Module

- Update libmagiskpolicy.so from Magisk (debug) 31.0 (31000)
- Prepare /storage/emulated/"$UID"/Android/data/$PKG/ directories
- Add New UI variant

v1.6 https://move2link.co/e193348
- Update apps from user-13-T1RAA33.39-11-2-ef936f-release-keys
- Using original maxx_conf.ini
- Check functions in mirror /apex files instead of mirror /system if exist
- Fix file permission & sepolicy denial

v1.5
- Support NoMount metamodule
- Update libmagiskpolicy.so from Magisk (stable) 30.7 (30700)
- Resets module folders/files permissions at post-fs-data
- Move _uninstall.log to /data/adb/logs/
- Removes conflicted weird modules
- Does not disable raw playback (You can use Audio Compatibility Patch Reborn Magisk Module instead)

v1.4
- Fix wrong target in latest KernelSU
- Improve detections

v1.3
- Tidy up aml.sh
- Exclude \*audio\*effects\*haptic\*.xml
- Abort installation if fail to mount mirror system
- Fix wrong file permissions in some ROMs
- Using libadspd.so built-in ROM if available

v1.2
- Improve /odm and /my_product support detection

v1.1
- Fix a crash

v1.0
- Fix BLUETOOTH_PRIVILEGED permission
- Add Action button to clear apps caches
- Fix architecture detection
- Fix bug in uninstall.sh
- Apply effect to rerouting and patch stream by default for game apps

v0.9
- Allow installation in Android Emulator
- Fix architecture detection

v0.8
- supportsAudioTuningForUsbHeadset=true
- launchMode="2" to fix not working togglers
- persistent="true" for quick settings tile responsiveness
- Improve \*audio\*effects\*xml patch detection
- Fix conflict with modules_update while installing via recovery if Magisk installed
- Fix architecture detection
- Fix MagiskHide & SUList
- Fix sepolicy denials

## Download Tutorial
https://t.me/ryukinotes/97

## Installation Guide
- If you are using KernelSU, you need to disable Unmount Modules by Default in KernelSU app settings and install https://github.com/KernelSU-Modules-Repo/meta-overlayfs or https://github.com/KernelSU-Modules-Repo/magic_mount_rs or https://github.com/KernelSU-Modules-Repo/hybrid_mount or https://github.com/maxsteeel/nomount first depending on ROM compatibility
- Remove any other else Moto Waves MAGISK MODULE with different name and reboot first (No need to remove if it's the same name)
- Install Moto Core Magisk Module first if using the original UI variant: https://github.com/reiryuki/Moto-Core-Magisk-Module except you are in Motorola ROM
- Install this module via Magisk app or Kitsune Mask app or KernelSU app or Apatch app or Recovery if Magisk or Kitsune Mask installed
- Install AML Magisk Module https://t.me/ryukinotes/34 only if using any other else audio mod module
- Reboot
- If you are using KernelSU, you need to allow superuser list manually all package name listed in package.txt (and your home launcher app also) (enable show system apps) and reboot afterwards
- If you are using SUList, you need to allow list manually your home launcher app (enable show system apps) and reboot afterwards
- For the original UI variant, open Audio effects app via quick settings and tap 'Show icon in the app tray' to show Audio effects app icon launcher
- For the original UI variant, tap 'About' then tap multiple times the version number there to show on/off toggler in loudspeakers mode

## Optionals
- https://t.me/ryukinotes/59
- Global: https://t.me/ryukinotes/35
- Stream: https://t.me/ryukinotes/52

## Troubleshootings
- https://t.me/ryukinotes/59
- Global: https://t.me/ryukinotes/34

## Support and Bug Report
- https://t.me/ryukinotes/54
- If you don't do above, issues will be closed immediately

## Known Issues
- Doesn't work with Bluetooth audio in ROM that doesn't support A2DP offload
- Doesn't work in some Android 14 (SDK 34) initial release (UP1A) nor QPR2 (AP1A) ROMs
- Doesn't work in some Android 15 (SDK 35) ROMs
- Looks like blobs not compatible with some Android 11 (SDK 30) ROMs

## Credits and Contributors
- @HuskyDG
- @Bobbyishere7
- https://t.me/viperatmos
- https://t.me/androidryukimodsdiscussions
- https://t.me/androidappsportdevelopment

## Sponsors and Donation
https://t.me/ryukinotes/25


