# brickfon_docs
Random dev stuff related to the myPhone Hammer Energy 2 ECO/Energy 2 2022
## TWRP
You can get the unofficial (and pretty janky) TWRP tree and (soon) builds [here](https://github.com/KZacharski/twrp-device-mptech-Energy_2_2022)
## Project Treble
Supports treble and dynamic partitions, VNDK 30. Can boot from both DSU sideloader and directly by flashing to system through fastbootd. For most GSIs it requires product to be removed to free up space on super. That doesn't affect the functionality of the phone. It's also affected by the mtk-related issue that breaks the system firewall on a12+ gsis causing it to block all connections even tho wifi/data appears to be working in settings. On a12-a14 this can be fixed with an adb command but on a15 the only way to fix it is patching the kernel which is impossible to do on this phone with already existing tools for this purpose. Currently there's no patches kernel available so Android 15 GSIs will have broken networking. Most GSIs don't boot on this device no matter the version, the only ones I managed to boot were various versions of LineageOS from AndyYan and MisterZtr.