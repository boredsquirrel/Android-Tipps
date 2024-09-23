# Debloat your phone

Manufacturers bloat your phone with software you dont want.

Android normally uses tightly sandboxed apps, which is why there are nearly no viruses. But systemapps have nearly full access to the system!

On low-end devices these system apps, running privileged and thus eating RAM, will cause other apps to crash.

So even if you want to keep apps, if they are on Appstores you should install them as a normal user app and not as a system app with full permissions over your whole system!

I.e. after uninstalling Youtube, you can install it as a regular user app from the playstore again. Maybe you need to use AuroraStore.


## Steps to do before:

1. Export your Contacts as a .vcf format. You need to visit your Google account on a Desktop browser to do that. Google Sucks. This offline Contact file can now be synced [using this app!](https://f-droid.org/en/packages/cx.vmx.sdcontacts). I recommend [Fossify Contacts](https://f-droid.org/de/packages/org.fossify.contacts).
2. Export your Calendar events. No idea how to do that, but using [DAVx5](https://f-droid.org/en/packages/at.bitfire.davdroid) and a CalDav provider like a good mail provider, you can have a great experience without Google lock-in.
3. Get your photos and files off the cloud. Use Cryptomator if you want to use cloud services you dont trust. Or just use [Syncthing](https://f-droid.org/en/packages/com.nutomic.syncthingandroid) with [Syncthingy on Linux](https://flathub.org/apps/com.github.zocker_160.SyncThingy) or SyncTrayzor on Windows. iOS and other crappy platforms are also supported, but you may need to pay.


## Things to consider

You phone will not be private after this.

On regular Android there are connections to
- Google for Internet connectivity check
- Google for A-GPS
- Google for Device ID, attestation, ...
- Often also your vendor
- Often Random 3rd parties your vendor made the OS with

The only thing that's partly secure is to use a custom DNS server blocking all the tracking, like NextDNS, and also NetGuard.

Note: System apps can bypass an "always on, block other connections" VPN. So NetGuard, Orbot or a privacy-friendly VPN do not apply here! Google still knows where you are, and so does any other system app that wants to. Another reason why you should have as little of them as possible (which is a core principle in GrapheneOS).

Android is not a private platform. It is an efficient, batterysaving, easy to build for Tracking Ecosystem. 

The only privacy friendly and secure Android is GrapheneOS, alternatives are DivestOS, LineageOS, CalyxOS, /e/OS etc. depending on your budget. If you have a Pixel, use GrapheneOS. If you have money, buy a (used) Pixel and install GrapheneOS on it. It is extremely easy.

Some Tricks:

## Disable instead of remove the Google triumvirate
Google Play Store, Play Services and Services Framework will cause constant error messages when uninstalled.

Instead, simply disable them.

```
pm disable --user 0 com.google.android.vending
pm disable --user 0 com.google.android.gsf
pm disable --user 0 com.google.anderoid.gms
```

(*not sure if those IDs are correct*)

## Disable debugging & developer options from the commandline

For security, or on quick mass device debloats, this can be handy.

```
settings put global development_settings_enabled 0
settings put global adb_enabled 0
```
## Reinstall an "uninstalled" system app
Mistakes happen, [here is how to do that](https://android.stackexchange.com/questions/215313/how-to-reinstall-an-uninstalled-system-app-through-adb):

```
adb shell
cmd package install-existing <package_name>
```
