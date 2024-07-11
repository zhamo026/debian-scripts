# debian-scripts
debian installation

after installing debian things to install

sudo apt update
sudo apt upgrade

sudo apt install flatpak snap neofetch

nano /home/lab/.bashrc  #add neofetch at the bottom

nano /home/lab/.config/neofetch/.config     #remove the hash from ip and usersave

Ctrl+O Crtl+X

sudo apt install openssh-server 


sudo systemctl start ssh

sudo systemctl enable ssh

sudo systemctl status ssh

nano /etc/ssh/sshd_config

unmark

#Port 22
#PermitRootLogin prohibit-password  change it to PermitRootLogin yes

Ctrl+O Crtl+X

service ssh restart

sudo apt remove firefox-esr

discovery
#remove libreoffice debianand reinstall the flathub verison
librewolf flatseal libreoffice 

remove libreoffice
sudo apt remove libreoffice-common libreoffice-core libreoffice-gnome libreoffice-gtk3 libreoffice-help-common libreoffice-help-en-us libreoffice-style-colibre libreoffice-style-elementary

intall extra codecs
sudo apt install libavcodec-extra


add a bacport repossitory and howto use
sudo nano /etc/apt/sources.list.d/backports.list
deb http://deb.debian.org/debian bookworm-backports main

deb http://deb.debian.org/debian bookworm-backports main
To install a package from that repository, add the -t option, like this:

sudo apt install -t bookworm-backports package-name 


add more repositories
sudo add-apt-repository contrib
sudo add-apt-repository non-free
sudo apt update


add headers
sudo apt install linux-headers-$(uname -r)


add esencials apps 
sudo apt install firmware-linux firmware-linux-nonfree vulkan-tools vulkan-validationlayers unrar gstreamer1.0-vaapi htop clang bpytop cargo libc6-i386 libc6-x32 libu2f-udev samba-common-bin exfat-fuse

 add java
sudo apt install default-jdk


battery saver
git clone https://github.com/AdnanHodzic/auto-cpufreq.git
ls
cd auto-cpufreq/
ls
sudo ./auto-cpufreq-installer
sudo systemctl status auto-cpufreq

install


minecraft
01. Log into the Debian device
   02. Run the following commands in a terminal window:
         update software repositories
         sudo apt update
         install java and flatpack
         sudo apt install openjdk-11-jdk flatpak gnome-software-plugin-flatpak
         add flatpack repo
         sudo flatpak remote-add --if-not-exists flathub https://flathub.org/repo/flathub.flat...
         install minecraft
         sudo flatpak install flathub com.mojang.Minecraft
         run minecraft
         flatpak run com.mojang.Minecraft
   03. Game!
