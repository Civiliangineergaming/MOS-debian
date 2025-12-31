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

backport:

deb http://deb.debian.org/debian trixie-backports main contrib non-free non-free-firmware

deb-src http://deb.debian.org/debian trixie-backports main contrib non-free non-free-firmware

sudo apt update

jak zainstalować pakiet z backport:

sudo apt install nazwa pakietu/trixie-backports

sudo apt install -t trixie-backports nazwa pakietu

