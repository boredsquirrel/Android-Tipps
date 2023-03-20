# Improve your privacy on stock Android with root

Rooting your phone is "daaangerous". If you use an insecure app, any app getting root privileges could run as superuser, which is basically what Windows and Linux look like by default.

So you see, it is very insecure and should be used sparely, but it works.
  
Only use secure, known and OpenSource tools on your phone, especially if its rooted.
  

## 1. [Install Magisk](https://topjohnwu.github.io/Magisk/install.html)
  
I won't copy everything here, visit the site for updated infos.
  
If your OS flash.zip Archive has a `payload.bin` inside, this means you can't get the needed `boot.img` immediately, which you need to reliable root your phone.
  
### 1.1 Get Payload dumper and unpack
  
requirements:

- Any Linux PC (or other OS capable of using `pip`)
- the payload.bin of your System
- The Magisk App installed on your phone, from F-Droid

run

```
pip install payload-dumper

payload-dumper ~/path/to/payload.bin
```

The resulting boot.img will end up in your ~/output folder (/home/username/output). Enable Data transfer in your phones connection settings and transfer this image to your phones storage.

### Modify the boot.img using Magisk
  
In the Magisk app modify the boot.img as said in the guide

### Flash the boot.img

You may need to run adb as root on your PC. Follow the Magisk guide. You see which slot you have booted in TWRP.
  
```
fastboot flash boot_a ~/magisk_patched-25200_sbrfb.img && fastboot boot ~/magisk_patched-NUMBER_sbrfb.img
```

works for Slot A.

# Useful modules

Get "Fox's Magisk module manager" to install Modules.

Lots of recent privacy fixes GrapheneOS applied to its Android are available as Magisk modules, as they are system changes that are not possilbe using normal Android apps.
  
  
- A-GPS SUPL replacer: Removes Google tracking even when only using A-GPS
- Magisk Captive Control (MCC): Allows removing or changing the Captive portal, otherwise always pinging Google
- Open Webview: Replaces Chromium WebView with Bromite Webview
- Mac Randomization Enabler: only for devices that dont support it, otherwise found in Developer Options
- Systemless Debloater: for rooted Stock Android
- Hide Userdebug, Test-Keys and LineageOS: May unbreak some apps detecting a custom ROM
- AppDataIsolation Legacy support: for old Android versions
- AFWall Boot Antileak: block internet access from blocked apps already on boot
- DNSCrypt-Proxy2: enables advanced DNScrypt modes

other useful tools

- F-Droid privileged Extension: Allows autoupdates from the F-Droid app
- Linux Chroot Installer
- Dalvik Hyperthreading: speed up your device
- Broadcomm speed up: increase your wifi speed
- Audio Misc: enable nicer audio settings
- Magisk DRM disabler: removes proprietary DRM, maybe breaks Netflix, Spotify & Co.
- fbind: many more mounting functions like encrypted LUKS drives and more
- ACC: protect your battery on devices not doing that already
- Move certificates: if you use an intercept or block proxy


And so much more.
  
Root is awesome! It gives users the freedom they deserve.
  
In a perfect world we wouldn't need root, but Google also wouldn't make Android.
