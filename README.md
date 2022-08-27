## HOW TO INSTALL NETHUNTER WITHOUT ROOT!!

# Installation:

- Install the NetHunter-Store app from [store.nethunter.com[(https://store.nethunter.com/)

- From the NetHunter Store, install Termux, NetHunter-KeX client, and Hacker's keyboard *Note: The button "install"
may not change to "installed" in the store client after installation - just ignore it. Starting termux for the first
time may seem stuck while displaying "installing" on some devices - just hit enter.*

- Open Termux and type:
```console
user@whatever:~$ termux-setup-storage
user@whatever:~$ pkg install wget
user@whatever:~$ wget -O install-nethunter-termux https://offs.ec/2MceZWr
user@whatever:~$ chmod +x install-nethunter-termux
user@whatever:~$ ./install-nethunter-termux
```

# Usage:

Open Termux and type one of the following:

![Usage Image](http://46.246.231.108/nethunter-rootless-usage.PNG)

# Tips:

1. Run ```console sudo apt update && sudo apt full-upgrade -y``` first thing after installation to update Kali. If you have plenty of storage space available you might want to run ```console sudo apt install -y kali-linux-default``` as well.
2. All of the penetration testing tools should work but some might have restrictions, e.g. ```console metasploit``` works but doesn’t have database support. If you discover any tools that don’t work, please post it in our forums.
3. Some utilities like “top” won’t run on unrooted phones.
4. Non-root users still have root access in the chroot. That’s a proot thing. Just be aware of that.
5. Galaxy phone’s may prevent non-root users from using sudo. Just ```console use su -c``` instead.
6. Perform regular backups of your rootfs by stopping all nethunter sessions and typing the following in a termux session: ```console tar -cJf kali-arm64.tar.xz kali-arm64 && mv kali-arm64.tar.xz storage/downloads``` That will put the backup in your Android download folder. Note: on older devices, change “arm64” to “armhf”
7. Please join us in our [forums](https://forums.kali.org/forumdisplay.php?14-NetHunter-Forums) to exchange tips and ideas and be part of a community that strives to make NetHunter even better.
