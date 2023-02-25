# Networking

\> ?  
\> sh ip int bri  
\> sh privi  
\> en  
\# exit  
\# conf t  
() do sh run  
() end  
() no ip domain-lookup  
\<CTRL\>\<SHIFT\>6  

() hostname \<name\>  
() banner motd \<char\> \<message\> \<char\>  
() line con 0  
(l) password \<password\>  
(l) login  
(l) no login  
() line vty 0 15  
(l) password \<password\>  
(l) no password  
(l) login  
() int vlan \<number\>  
(i) ip add \<ip\> \<mask\>  
(i) shutdown  
(i) no shutdown  
() enable password \<password\>  
ping \<ip\>  
telnet \<ip\>  
() ip default-gateway \<ip\>  
\# write  
\# copy running-config startup-config  
() ip domain-name <domain>  
() crypto key generate rsa  
1204  
() ip ssh version 2  
() username \<username\> password \<password\>  
() line vty 0 15  
(l) transport input none  
(l) transport input shh  
(l) login local  
ssh -l \<username\> \<ip\>  
\<password\>  

(i) switchport mode access  
(i) switchport mode trunk  
(i) switchport mode dynamic desirable  
(i) switchport mode dynamic auto  
(i) switchport mode nonegotiate  

() int gi0/0  
() router rip  
  
