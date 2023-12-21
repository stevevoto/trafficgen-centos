# trafficgen-centos
1. Download and install the CentOS-7-min http://mirror.metrocast.net/centos/7.9.2009/isos/x86_64/CentOS-7-x86_64-Minimal-2009.iso
2. **ssh** to your device with your username/passwd and sudu su to root
3. Connect your Desktop to the internet and make sure **DNS** is configured properly
4. IMPORTANT you must run " ***yum -y install wget** " as root from linux to download the installer.
5. From Linux download **wget** https://github.com/stevevoto/trafficgen-centos/raw/main/CentOsTrafficGenerator.sh
7. After downloading type " **chmod +x CentOsTrafficGenerator.sh** "
8. Run **./CentOsTrafficGenerator.sh**
9. When Complete the server will **reboot**
10. Login as root
11. When reboot is complete check service is runnning "sudo systemctl status web-traffic-gen.service"
12. If services is not running run the following command: sudo systemctl start web-traffic-gen.service
13. If service is runnining you can do a tcpdump and watch connections
