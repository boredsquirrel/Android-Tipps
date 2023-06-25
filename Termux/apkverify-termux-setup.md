## Verify downloaded APK Signatures on your Android phone
Using Termux you can use a complete Linux system on your Android device. This means my tool "apkverify" should also work on Android.

Currently there are some errors I need to find the reason for.

## 1. Install apps

`pkg install -y fish apksigner wget curl tldr unzip`

## 2. Shell configs

### 2.1 Bash config

```
cat >> ~.bashrc <<EOF

###### CUSTOM #######
alias up='pkg update -y && pkg upgrade -y && echo "Done"

alias conf='nano ~/.bashrc && . ~/.bashrc && echo 

alias reload='. ~/.bashrc' && echo "Bashrc reloaded"

### NETWORKING
alias myip='curl ifconfig.co'
alias netlisten='netstat -plntu'
alias pingtest='ping -c 2 wikipedia.de'

alias httpcode="curl --head --silent --output /dev/null --write-out '%{http_code}' "

alias "q"="exit"
alias c="clear"

 # List (ls)
alias ll='ls -alF'
alias la='ls -A'
alias l='ls -CFl'
alias ls="ls --color=auto"

alias f=fish

PATH="${PATH:+${PATH}:}~/.bin:~/.local/bin:~/.cargo/bin"

#automatically move to Android home dir
cd /storage/emulated/0

EOF
```

### 2.2 Fish config
```
cat >> ~.config/fish/config.fish <<EOF

###### CUSTOM #########
alias up='pkg update -y && pkg upgrade -y && echo "Done"

alias conf='nano ~/.bashrc && . ~/.bashrc && echo 

alias reload='. ~/.bashrc' && echo "Bashrc reloaded"

alias mkdir='mkdir -v'

### NETWORKING
alias myip='curl ifconfig.co'
alias netlisten='netstat -plntu'
alias pingtest='ping -c 2 wikipedia.de'

alias httpcode="curl --head --silent --output /dev/null --write-out '%{http_code}' "


alias "q"="exit"
alias c="clear"

 # List (ls)
alias ll='ls -alF'
alias la='ls -A'
alias l='ls -CFl'

set PATH $PATH ~/.bin ~/.local/bin ~/.cargo/bin

cd /storage/emulated/0

EOF
```

## 3. Apkverify

```
mkdir ~/.bin
wget https://raw.githubusercontent.com/trytomakeyouprivate/Android-Tipps/main/APK-Signer/apkverify -P ~/.bin
chmod +x ~/.bin/apkverify
```

