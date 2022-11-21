__Software__:
-VM
-Windows 10 ISO
-Server 9 ISO

__VM Server__

`Internal`
-Network Interface Card => Internet
-DHCP will self assign from home router

`External`
-Network Interface Card => VM Network
-IP: 172.16.0.1 // Private Class B
-Mask: 255.255.255.0 // Class C Subnet
-Gateway: Empty
-DNS: 127.0.0.1 // Local Host Ping

