Debloat 

```
adb shell
pm uninstall --user 0 com.google.android.apps.enterprise.dmagent
pm uninstall --user 0 com.google.android.launcher.layouts.bullhead
pm uninstall --user 0 com.android.hotwordenrollment
pm uninstall --user 0 com.google.android.launcher
pm uninstall --user 0 com.google.android.deskclock
pm uninstall --user 0 com.google.android.music
pm uninstall --user 0 com.google.android.apps.cloudprint
#pm uninstall --user 0 com.android.cellbroadcastreceiver
pm uninstall --user 0 com.android.facelock
pm uninstall --user 0 com.google.android.gm.exchange
pm uninstall --user 0 com.google.android.calculator
pm uninstall --user 0 com.google.android.tag
pm uninstall --user 0 com.verizon.omadm
pm uninstall --user 0 com.google.android.apps.walletnfcrel
pm uninstall --user 0 com.google.android.feedback
pm uninstall --user 0 com.google.android.gsf.login
pm uninstall --user 0 com.google.android.backuptransport
pm uninstall --user 0 com.google.android.apps.tycho
pm uninstall --user 0 com.google.android.talk
pm uninstall --user 0 com.google.android.apps.gcs
pm uninstall --user 0 com.google.android.GoogleCamera
```

Hard debloat (will break things)

```
pm uninstall --user 0 com.google.android.gms
pm uninstall --user 0 com.google.android.gsf
```

Apps you may want

```
pm uninstall --user 0 com.google.android.dialer
pm uninstall --user 0 com.google.android.launcher
pm uninstall --user 0 com.google.android.apps.inputmethod.hindi
pm uninstall --user 0 com.google.android.inputmethod.korean
pm uninstall --user 0 com.google.android.inputmethod.pinyin
pm uninstall --user 0 com.google.android.inputmethod.japanese
```
