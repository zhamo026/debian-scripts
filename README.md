# debian-scripts
debian installation

after installing debian things to install

sudo apt update
sudo apt upgrade

sudo apt install flatpak snap neofetch

nano /home/lab/.bashrc  #add neofetch at the bottom

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

