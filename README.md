dodanie urzytkownika do grupy sudo:

su -

usermod -aG sudo nazwa_uzytkownika

reboot

dodanie repozytoriów:

sudo nano /etc/apt/sources.list

zwykłe repozytoria:

deb http://deb.debian.org/debian/ trixie main non-free-firmware

deb-src http://deb.debian.org/debian/ trixie main non-free-firmware

deb http://security.debian.org/debian-security trixie-security main non-free-firmware

deb-src http://security.debian.org/debian-security trixie-security main non-free-firmware

deb http://deb.debian.org/debian/ trixie-updates main non-free-firmware

deb-src http://deb.debian.org/debian/ trixie-updates main non-free-firmware

sudo apt update

testing:

deb http://deb.debian.org/debian testing main non-free non-free-firmware

deb-src http://deb.debian.org/debian testing main non-free non-free-firmware

sudo apt update

unstable:

deb http://deb.debian.org/debian unstable main non-free non-free-firmware

deb-src http://deb.debian.org/debian unstable main non-free non-free-firmware

sudo apt update
