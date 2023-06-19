# apkverify

This little tool helps you verify, that an Android app is safe to install.

Luckily this works without extra PGP-Keys and everything.

## Installation

```
mkdir ~/.bin
wget https://raw.githubusercontent.com/trytomakeyouprivate/Android-Tipps/main/APK-Signer/apkverify -P ~/.bin
chmod +x ~/.bin/apkverify
```
`
# Example output:
```
user@machine ❯❯❯ apkverify shelter-github.apk

===== APK Signer Output =====

Verified using v2 scheme (APK Signature Scheme v2): true

===== Certificate Output =====

Eigentümer: CN=Peter Cai
Aussteller: CN=Peter Cai
Seriennummer: 6dcab902
Gültig von: Thu Aug 23 14:03:07 CEST 2018 bis: Sat Jul 30 14:03:07 CEST 2118
Zertifikatsfingerprints:
         SHA1: 7A:1E:07:07:F9:B9:73:20:3A:6D:A4:4F:84:44:E5:A8:74:04:4D:20
         SHA256: D7:3D:3C:71:5B:DE:7F:C8:6C:1C:15:6F:F3:D5:73:CF:8B:9C:67:0F:5A:1F:3C:5E:F8:23:BE:40:E6:05:29:8A
Signaturalgorithmusname: SHA256withRSA
Public Key-Algorithmus von Subject: 2048-Bit-RSA-Schlüssel
Version: 3

Erweiterungen: 

#1: ObjectId: 2.5.29.14 Criticality=false
SubjectKeyIdentifier [
KeyIdentifier [
0000: DD E0 20 37 AF 98 4C 88   C0 95 EC 0E E3 3C A1 C0  .. 7..L......<..
0010: B8 4C 60 05                                        .L`.
]
]
```

## Dependencies
It uses apksigner and keytool to print the information.

make sure `~/.bin` is an existing directory and in your $PATH

## OS-Dependency
Apksigner is only available on Ubuntu, you can use it through distrobox:

```
distrobox create Ubuntu -i docker.io/library/ubuntu:22.04 && \
distrobox enter Ubuntu
```

```
sudo apt install -y apksigner && \
distrobox-export --bin /usr/bin/apksigner --export-path ~/.bin/
```

## Detailed explanation
See the comments in the script
