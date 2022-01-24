# mint-pulse

sudo apt update
sudo apt upgrade
sudo apt full-upgrade
sudo apt dist-upgrade
sudo apt autoremove
sudo apt autoclean
sudo apt clean
sudo reboot (Reinicializar o Sistema)

#08_ Instalação do Linux Kernel OEM (versão do Kernel instalada >= 5.10.x suportado até 2025)

sudo apt update
sudo uname -a
sudo apt install linux-oem-20.04 fdutils
sudo reboot (Reinicializar o Sistema)

#09_ Instalação dos Aplicativos Básicos

sudo apt update
sudo apt install software-properties-common build-essential lsb-core dkms
sudo apt install htop nmon i8kutils psensor tlp tlp-rdw cpufrequtils cputool
sudo apt install ttf-mscorefonts-installer cheese guvcview cairo-dock vim git p7zip-full p7zip-rar
sudo reboot (Reinicializar o Sistema)


#INSTALACAO DA VPN
sudo apt install wireguard
sudo apt install resolvconfig

sudo cp wg0.conf /etc/wireguard
sudo systemctl enable wg-quick@wg0
sudo systemctl start wg-quick@wg0.service
sudo systemctl status wg-quick@wg0.service

#CHAVE SSH para o https://gitlab.mateus

sudo ssh-keygen -t rsa -C zeuxis.silva@grupomateus.com
