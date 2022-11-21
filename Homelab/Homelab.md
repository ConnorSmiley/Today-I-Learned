__Software__:
-VM
-Windows 10 ISO
-Server 9 ISO

__VM Server__

`Internet NIC`
-Network Interface Card => Internet
-DHCP will self assign from home router

`Internal NIC`
-Network Interface Card => VM Network
-IP: 172.16.0.1 // Private Class B
-Mask: 255.255.255.0 // Class C Subnet
-Gateway: Empty
-DNS: 127.0.0.1 // Local Host Ping
-Server 9 for IP addressing

__Active Directory__
-Create Domain

__NAT__
`Network Address Translation`
-Setup NAT

__DHCP__
-Range: 172.16.0.100-200
-Mask: 255.255.255.0 // Class C Subnet
-Gateway: 172.168.0.1
-DNS: 172.16.0.1




