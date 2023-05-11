# Debloat your phone

Manufacturers bloat your phone with software you dont want.

Android normally uses containerized apps, which is why there are nearly no viruses. But systemapps are not containerized!

So even if you want to keep apps, if they are on Appstores you should install it as a normal user app and not as a system app with full permissions over your whole system!


## Steps to do before:

1. Export your Contacts as a .vcf format. You need to visit your Google account on a Desktop browser to do that. Google Sucks. This offline Contact file can now be synced [using this app!](https://f-droid.org/en/packages/cx.vmx.sdcontacts). I recommend "Simple Contacts Pro"
2. Export your Calendar events. No idea how to do that, but use your own provider using [DAVx5](https://f-droid.org/en/packages/at.bitfire.davdroid) and a CalDav provider like a good mail provider, not google
3. Get your photos and files off the cloud. Use Cryptomator if you want to use services you dont trust. Or just use [Syncthing](https://f-droid.org/en/packages/com.nutomic.syncthingandroid) with [Syncthingy on Linux](https://flathub.org/apps/com.github.zocker_160.SyncThingy) or SyncTrayzor on Windows. Just iOS is not supported


## Things to consider

You phone will not be private after that. 

On regular Android there are connections to
- Google for Internet connectivity check
- Google for A-GPS
- Google for Device ID
- lots more
- your manufacturer

The only thing thats partly secure is to use a custom DNS server blocking all the tracking, like NextDNS, and also NetGuard.

Note: System apps can bypass an "always on, block other connections" VPN.

Android is not a private platform.

The only privacy friendly OS is GrapheneOS.
