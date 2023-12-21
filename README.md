# trafficgen-centos
Download and install the CentOS-7-min located here [https://releases.ubuntu.com/18.04/ubuntu-18.04.6-desktop-amd64.iso.](http://mirror.metrocast.net/centos/7.9.2009/isos/x86_64/CentOS-7-x86_64-Minimal-2009.iso)
ssh to your device with your username/passwd and sudu su to root
Connect your Desktop to the internet and make sure DNS is configured properly
From Linux with root privledges download this installer. 
When Complete the server will reboot
Login as root
When Complete check service is runnning "sudo systemctl status web-traffic-gen.service"
If services is not running run the following command: sudo systemctl start web-traffic-gen.service
If service is runnining you can do a tcpdump and watch connections
