#!/bin/sh
#--------------Web Traffic Generator Centos7 -------
sudo yum install -y dnf
sudo dnf -y install openssh-server
sudo dnf -y install git curl
sudo yum -y install epel-release wget net-tools lshw ntp tcpdump iperf iperf3 git tcpdump htop 
sudo yum groups -y install "GNOME Desktop"
sudo systemctl set-default graphical.target
sudo systemctl start graphical.target
wget https://dl.google.com/linux/direct/google-chrome-stable_current_x86_64.rpm
sudo yum -y install google-chrome-stable_current_x86_64.rpm
cd /etc/yum.repos.d/
wget https://github.com/stevevoto/trafficgen-centos/raw/main/nodesource-el.repo
dnf makecache
sudo yum install -y nodejs
cd ~
git clone https://github.com/stevevoto/trafficGen.git
cd trafficGen/
chmod +x install.sh 
sudo ./install.sh
sudo chmod 755 /usr/bin/traffgen 
sudo systemctl start web-traffic-gen.service
sudo systemctl status web-traffic-gen.service
sudo systemctl enable web-traffic-gen.service
sudo reboot now
