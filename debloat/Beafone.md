Debloat

```
adb shell
pm uninstall --user 0 com.android.egg #EasterEgg
#pm uninstall --user 0 com.google.android.apps.restore #Restore Apps with Google account, Tracking
pm uninstall --user 0 com.google.android.apps.googleassistant
pm uninstall --user 0 com.mediatek.autodialer
#pm uninstall --user 0 com.android.callogbackup
pm uninstall --user 0 com.google.android.ims
pm uninstall --user 0 com.android.chrome
pm uninstall --user 0 com.mediatek.gnssdebugreport #https://geekloving.net/de/so-entfernen-sie-oppo-system-apps-ohne-root#Mediatek_Bloatware_auf_Oppo
pm uninstall --user 0 se.dirac.acs
pm uninstall --user 0 com.trustonic.teeservice
pm uninstall --user 0 com.mediatek.mdmlsample
pm uninstall --user 0 com.google.android.overlay.searchlauncherconfig
pm uninstall --user 0 com.google.android.apps.wellbeing #tracking
pm uninstall --user 0 com.google.android.apps.docs #Drive
pm uninstall --user 0 com.google.android.apps.tachyon #Google Duo
pm uninstall --user 0 com.facebook.katana
pm uninstall --user 0 com.google.android.apps.nbu.files
pm uninstall --user 0 com.google.android.apps.photos
pm uninstall --user 0 com.google.android.gm #Gmail
pm uninstall --user 0 com.google.android.googlequicksearchbox
#pm uninstall --user 0 com.google.android.onetimeinitializer
#pm uninstall --user 0 com.google.android.partnersetup
pm uninstall --user 0 com.google.android.play.games
pm uninstall --user 0 com.google.android.videos
pm uninstall --user 0 com.google.android.syncadapters.contacts #Kontakt-Sync with Google servers, yay
pm uninstall --user 0 com.google.android.gms.location.history
#pm uninstall --user 0 com.android.location.fused #network location service?
pm uninstall --user 0 com.google.android.apps.maps
pm uninstall --user 0 com.google.android.apps.messaging #Google SMS
pm uninstall --user 0 com.evelynforpps.newpipehelp
pm uninstall --user 0 com.shaiban.audioplayer.mplayer #3rd party music
pm uninstall --user 0 com.v.smartassistant.outdoortool
pm uninstall --user 0 com.teamviewer.quicksupport.market #teamviewer, REMOVE
pm uninstall --user 0 com.vanzo.sos
pm uninstall --user 0 com.google.android.apps.setupwizard.searchselector
pm uninstall --user 0 com.fineos.superscreenshot
pm uninstall --user 0 com.zzaudiotube04.mp4.video.downloader
pm uninstall --user 0 com.wapi.wapicertmanager #shady
pm uninstall --user 0 com.mediatek.ygps #high battery drain
pm uninstall --user 0 com.google.android.youtube
pm uninstall --user 0 com.google.android.apps.youtube.music
pm uninstall --user 0 com.loudtalks

```

Hard debloat (Will break things)

```
pm uninstall --user 0 com.android.vending #Playstore
pm uninstall --user 0 com.google.android.gms #Google Play Services
pm uninstall --user 0 com.google.android.gsf #Google services framework
pm uninstall --user 0 com.android.bookmarkprovider
pm uninstall --user 0 com.mediatek.ims #maybe important
pm uninstall --user 0 com.sprd.screencapture
pm uninstall --user 0 com.mediatek.duraspeed #maybe important for battery
```

Apps you may want

```
pm uninstall --user 0 com.google.android.projection.gearhead #Android Auto
pm uninstall --user 0 com.google.android.marvin.talkback #Accessibility
pm uninstall --user 0 com.google.android.calendar
pm uninstall --user 0 com.mediatek.camera
pm uninstall --user 0 com.google.android.tts #Speech services by google
```
