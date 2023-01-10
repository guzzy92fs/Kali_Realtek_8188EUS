1. sudo su 
2. apt update 
3. apt upgrade 
4. apt  install dkms
5. git clone https://github.com/aircrack-ng/rtl818... 
6. cd rtl8188eus 
7. make && sudo make install 
8. echo 'blacklist r8188eu'|sudo tee -a '/etc/modprobe.d/realtek.conf' 9. reboot 

Monitor Mode Command:  


1. sudo su 
2. airmon-ng check kill 
3. ip link set (interface) down 
4. iw dev (interface) set type monitor
5. service NetworkManager restart 

Monitor Mode Test Command: 

1. airodump-ng (interface) 
2. Wifite  

Managed Mode Command:  

1. sudo su  
2. airmon-ng check kill 
3. ip link set (interface) down 
4. iw dev (interface) set type managed 
5. service NetworkManager restart   

"make && sudo make install" 
After This Command Getting This Error ( SOLVED)  
"cut: /etc/redhat-release: No such file or directory make ARCH=x86_64 CROSS_COMPILE= -C /lib/modules/5.14.0-kali4-amd64/build M=/root/Desktop/rtl8188eus  
modules make[1]:  * /lib/modules/5.14.0-kali4-amd64/build: No such file or directroy.    
Stop. make: * [makefile:2062: module] Error 2" 


** Use This This Two Commands  ** 

"apt install bc" 
"apt install dkms"
