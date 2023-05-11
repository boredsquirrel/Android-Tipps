Note: other general debloating already applied

```
adb shell
pm uninstall --user 0 com.adobe.reader
pm uninstall --user 0 com.android.egg
pm uninstall --user 0 com.google.android.ims
pm uninstall --user 0 com.android.chrome
pm uninstall --user 0 com.mediatek.duraspeed
pm uninstall --user 0 com.mediatek.ims
pm uninstall --user 0 com.google.android.apps.wellbeing
pm uninstall --user 0 com.google.android.apps.docs
pm uninstall --user 0 com.google.android.apps.nbu.files
pm uninstall --user 0 com.google.android.apps.photosgo
pm uninstall --user 0 com.mediatek.gb
pm uninstall --user 0 com.elephnttek.faceunlock
pm uninstall --user 0 com.google.android.apps.assistant
pm uninstall --user 0 com.google.android.apps.searchlite
pm uninstall --user 0 com.google.android.gmsintegration
pm uninstall --user 0 com.google.android.calendar
pm uninstall --user 0 com.mediatek.camera
pm uninstall --user 0 com.android.location.fused #potentially very invasive
pm uninstall --user 0 com.google.android.contacts
pm uninstall --user 0 com.google.android.apps.youtube.music
```

Hard debloat (Will break things)

```
pm uninstall --user 0 com.google.android.inputmethod.latin
pm uninstall --user 0 com.google.android.apps.speechservices
pm uninstall --user 0 com.google.android.gsf #Google servicec framework
pm uninstall --user 0 com.android.vending #Google Play
pm uninstall --user 0 com.google.android.gms
```

Apps you may want

```
pm uninstall --user 0 com.spotify.music
pm uninstall --user 0 fr.vinted
```
