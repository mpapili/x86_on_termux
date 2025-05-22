# x86_on_termux
hopefully not much more than a readme and a shell script

## ssh into your phone (optional, but keeps me sane)
in termux
```bash
pkg install openssh -y
```

determine your user
```bash
whoami
```
set a password (note - DO NOT LEAVE SSH AUTO-ENABLED IF YOU USE PASSWORD AUTH!)
```bash
passwd
```

start ssh server
```bash
sshd -p 8081
```

find your IP address on the local network
```bash
ifconfig
```
(search for wlan)

then from your host machine
```bash
ssh <username_you_found>@<ip_you_found> -p 8081
```
