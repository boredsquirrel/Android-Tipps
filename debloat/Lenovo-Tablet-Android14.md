## Lenovo Tablet debloat

```
adb shell
```

apps you may want
```
pm disable --user 0 com.google.android.apps.adm #find my device
pm disable --user 0 com.google.android.apps.chromecast.app
pm disable --user 0 com.google.android.apps.satetyhub
```

untested
```
pm disable --user 0 com.google.android.adservices.api #data protection on advertizing?
pm disable --user 0 com.lenovo.lsf
pm disable --user 0 com.myscript.nebo.lenovo
pm disable --user 0 com.tblenovo.tabpushout
pm disable --user 0 com.zui.camera.qr #lenovo camera qr scanner
pm disable --user 0 com.zui.keyboardupdate #Firmware update for the keyboard???
pm disable --user 0 com.zui.recorder
pm disable --user 0 com.zui.wifip2p #zui one?
pm disable --user 0 com.huaqin.NvService # no idea what that is
```

```
pm disable --user 0 com.android.chrome
pm disable --user 0 com.google.android.inputmethod.latin #gboard
pm disable --user 0 com.google.android.youtube
pm uninstall --user 0 cn.wps.moffice_eng
pm uninstall --user 0 com.android.hotwordenrollment.okgoogle
pm uninstall --user 0 com.android.hotwordenrollment.xgoogle
pm uninstall --user 0 com.google.android.apps.books
pm uninstall --user 0 com.google.android.apps.docs
pm uninstall --user 0 com.google.android.apps.googleassistant
pm uninstall --user 0 com.google.android.apps.kids.home
pm uninstall --user 0 com.google.android.apps.magazines
pm uninstall --user 0 com.google.android.apps.maps
pm uninstall --user 0 com.google.android.apps.messaging
pm uninstall --user 0 com.google.android.apps.subscriptions.red
pm uninstall --user 0 com.google.android.apps.tachyon #google meet
pm uninstall --user 0 com.google.android.apps.wellbeing
pm uninstall --user 0 com.google.android.apps.youtube.music
pm uninstall --user 0 com.google.android.apps.youtube.music.setupwizard
pm uninstall --user 0 com.google.android.as #android system intelligence
pm uninstall --user 0 com.google.android.calendar
pm uninstall --user 0 com.google.android.contacts
pm uninstall --user 0 com.google.android.deskclock #uhr
pm uninstall --user 0 com.google.android.gm #gmail
pm uninstall --user 0 com.google.android.gms.location.history
pm uninstall --user 0 com.google.android.googlequicksearchbox
pm uninstall --user 0 com.google.android.healthconnect.controller #health connect
pm uninstall --user 0 com.google.android.photos ########### instead fossify gallery or aves
pm uninstall --user 0 com.google.android.play.games
pm uninstall --user 0 com.google.android.tts
pm uninstall --user 0 com.google.android.videos
pm uninstall --user 0 com.lenovo.weathercenter
pm uninstall --user 0 com.mediatek.location.lppe.main
pm uninstall --user 0 com.motorola.demo #demo modus
pm uninstall --user 0 com.motorola.mobiledesktop
pm uninstall --user 0 com.myscript.calculator.lenovo
pm uninstall --user 0 com.opera.browser
pm uninstall --user 0 com.opera.preinstall
pm uninstall --user 0 com.tblenovo.center #lenovo vantage
pm uninstall --user 0 com.tblenovo.lenovowhatsnew
pm uninstall --user 0 com.zui.camera.asisstant #camera assistant, instagram logo?
pm uninstall --user 0 com.zui.notes
pm uninstall --user 0 com.zui.recorder
pm uninstall --user 0 com.zui.udevice
pm uninstall --user 0 com.zui.uface ###?
pm uninstall --user 0 com.zui.weather
pm uninstall --user 0 com.google.android.apps.photos
pm uninstall --user 0 com.google.android.apps.mediahome.launcher
pm uninstall --user 0 com.google.android.apps.walletnfcrel # google wallet
pm uninstall --user 0 com.zimi.weather
pm uninstall --user 0 com.google.android.apps.podcasts
```
