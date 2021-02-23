# Lenovo-Ideapad-320-15ikb-Hacintosh

Disclaimer

Your warranty is now void. Please do some research if you have any concerns before replacing your EFI with mine. I am not responsible for any loss, including but not limited to Kernel Panic, device fail to boot or can not function normally, storage damage or data loss, atomic bombing, World War III and so on.


A guide for installing macOS Big Sur and Catalina and below on Lenovo IdeaPad 320-15IKB using Opencore 


# Laptop's Hardware 

| Name       | Specifications         | Funtional or not  |
| ------------- |:-------------:| -----:|
| Processor     | Intel Core i5-7200U Processor | Fully  |
| Memory     |8GB LPDDR4 2133MHz|  Fully  |
| Storage |  2TB Seagate Hdd    |  Fully  |
|   Graphics   |  Intel HD Graphics 620| Fully with WhateverGreen.kext and properties inject|
|Display|  13.9" FHD 1920x1080 LED IPS    |  Fully |
| Audio |  Realtek Audio ALC230 codec     |  Fully with AppleALC.kext   |
|   Ethernet   | Intel(R) Ethernet Connection  | Fully with IntelMausi.kext |
|   WLAN & Bluetooth   |  Intel 3165     |  Fully with Airportitlwm  |
| Ports|  1 x USB-C, 2 x USB 3.0,USB 2.0 SD Card Reader, HDMI Display Port     | Fully with USBPorts.kext    |
| Trackpad   | TrackPoint and multi-touch touchpad |  Fully with VoodooPS2Controller.kext |
|  Keyboard    | Generic Lenovo Keyboard      |  Fully  |


# Note 
 * Display-- The model of Integrated Graphics is Intel UHD Graphics 620, faked to Intel HD Graphics 620. VRAM has been set to 3072 MB.
 * HDMI-- HDMI port (including HDMI Audio) is supported.
 * Sleep--Sleep (hibernation, lid sleep, and lid wake) is working fine.
 
 
 
 
 
# BIOS Configuration

Before doing anything, make sure to update your BIOS to the latest version from here, preparing your laptop to macOS, reboot your laptop, when the Lenovo logo appears press F2, when the BIOS menu appears go to:

* "Configuration" SATA Controller Mode to AHCI, HotKey Mode to Enabled.
* "Security" Intel Platform Trust Technology to Disabled, Intel SGX to Disabled, Secure Boot to Disabled.
* "Boot" Boot Mode to UEFI,Fast Boot to Disabled, USB Boot to Enabled.
* "Exit" OS Optimized Defaults to Disabled.


# What's Not Working.

Apple Pay, requires TouchID,(not supported since this Laptop does not have ApplePay Hardware.

Requirement

16GB USB drive or higher.
macOS Big Sur/Catalina image downloaded from the Appstore.

# Credits

* Apple for macOS.
* Acidanthera for most of the kexts.
* RehabMan for some ACPI patches.
* Steve Zheng for some patches.
* zhen-zen for YogaSMC.
* Hiep Bao Le for AppleBacklightSmoother
Thanks to all the Developers who made this Hacintosh possible.


