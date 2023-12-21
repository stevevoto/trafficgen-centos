# trafficgen-centos
1. Download and install the CentOS-7-min located here http://mirror.metrocast.net/centos/7.9.2009/isos/x86_64/CentOS-7-x86_64-Minimal-2009.iso
2. ssh to your device with your username/passwd and sudu su to root
3. Connect your Desktop to the internet and make sure DNS is configured properly
4. From Linux with root privledges download this installer. "wget https://github.com/stevevoto/trafficgen-centos/raw/main/web-traff-gen"
5. After downloading type "chmod +x web-traff-gen.sh" 
6. When Complete the server will reboot
7. Login as root
8. When reboot is complete check service is runnning "sudo systemctl status web-traffic-gen.service"
9. If services is not running run the following command: sudo systemctl start web-traffic-gen.service
10. If service is runnining you can do a tcpdump and watch connections
