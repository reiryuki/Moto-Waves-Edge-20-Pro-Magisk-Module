# Moto Waves V2 Edge 20 Pro Magisk Module

## DISCLAIMER
- Motorola and Waves apps and blobs are owned by Motorola™ and Waves™.
- The MIT license specified here is for the Magisk Module only, not for Motorola and Waves apps and blobs.

## Descriptions
- Equalizer sound effect ported from Motorola Edge 20 Pro (pstar) and integrated as a Magisk Module for all supported and rooted devices with Magisk
- Global type sound effect

## Sources
- https://dumps.tadiphone.dev/dumps/motorola/pstar user-13-T1RA33.55-15-10-72f29-release-keys
- system_support: LineageOS ROM Android 14
- libmagiskpolicy.so: Magisk (stable) 30.7 (30700)

## Changelog

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
- Fix selinux denials

v0.7
- Add miui.intent.action.HEADSET_SETTINGS

v0.6
- Fix installation failure caused by function not found
- Fix a fatal exception & auto reboot in Android 14
- Redirect /sdcard to /data/media/"$UID"
- Add new Magisk and Kitsune Mask support (independent mirror)
- Remount partitions before mounting mirror to prevent mount failure caused by device/resource busy
- Sets system property ro.audio.monitorWindowRotation=true if audio.rotation=1 at optionals.prop
- Fix MagiskHide & SUList
- Kitsune Mask detection

## Screenshots
https://t.me/androidryukimods/1063

## Requirements
- armeabi-v7a or arm64-v8a with armeabi-v7a support architecture
- 32 bit HIDL audio service
- Android 11 (SDK 30) until 14 (SDK 34) only
- Magisk or Kitsune Mask or KernelSU or Apatch installed
- Moto Core Magisk Module installed https://github.com/reiryuki/Moto-Core-Magisk-Module except you are in Motorola ROM
- Bluetooth A2DP offload ROM support for Bluetooth audio

## Installation Guide & Download Link
- If you are using KernelSU, you need to disable Unmount Modules by Default in KernelSU app settings and install https://github.com/KernelSU-Modules-Repo/meta-overlayfs or https://github.com/KernelSU-Modules-Repo/magic_mount_rs or https://github.com/KernelSU-Modules-Repo/hybrid_mount or https://github.com/maxsteeel/nomount first depending on ROM compatibility
- Remove any other else Moto Waves MAGISK MODULE with different name and reboot first (No need to remove if it's the same name)
- Install Moto Core Magisk Module first: https://github.com/reiryuki/Moto-Core-Magisk-Module except you are in Motorola ROM
- Install this module via Magisk app or Kitsune Mask app or KernelSU app or Apatch app or Recovery if Magisk or Kitsune Mask installed
- Install AML Magisk Module https://t.me/ryukinotes/34 only if using any other else audio mod module
- Reboot
- If you are using KernelSU, you need to allow superuser list manually all package name listed in package.txt (and your home launcher app also) (enable show system apps) and reboot afterwards
- If you are using SUList, you need to allow list manually your home launcher app (enable show system apps) and reboot afterwards
- Open Moto Audio app via quick settings and tap 'Show icon in the app tray' to show Moto Audio app icon launcher
- Tap 'About' then tap multiple times the image if you want to disable effect for loudspeaker

## Optionals
- https://t.me/ryukinotes/59
- Global: https://t.me/ryukinotes/35
- Stream: https://t.me/ryukinotes/52

## Troubleshootings
- https://t.me/ryukinotes/59
- Global: https://t.me/ryukinotes/34

## Support & Bug Report
- https://t.me/ryukinotes/54
- If you don't do above, issues will be closed immediately

## Known Issues
- Doesn't work with Bluetooth audio in ROM that doesn't support A2DP offload
- Doesn't work in Android 14 (SDK 34) initial release (UP1A) nor QPR2 (AP1A)
- Looks like blobs not compatible with Android 11 (SDK 30)

## Credits and Contributors
- @HuskyDG
- https://t.me/viperatmos
- https://t.me/androidryukimodsdiscussions
- You can contribute ideas about this Magisk Module here: https://t.me/androidappsportdevelopment

## Sponsors
https://t.me/ryukinotes/25


