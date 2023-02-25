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
(i) no sh  
() enable password \<password\>  
ping \<ip\>  
telnet \<ip\>  
() ip default-gateway \<ip\>  
\# write  
\# copy running-config startup-config  
() ip domain-name <name>  
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
\# show mac address-table  

(i) switchport mode access  
(i) switchport mode trunk  
(i) switchport mode dynamic desirable  
(i) switchport mode dynamic auto  
(i) switchport mode nonegotiate  
() vtp mode \<server/client/transparent\>  

\# sh vlan  
() vlan \<number\>  
(v) name \<name\>  
() int f0/1  
() int range f0/2-3  
(i) switchport mode access  
(i) switchport access vlan \<number\>  

() vtp pruning  
() int \<interface\>  
(i) switchport mode trunk  
(i) switchport trunk allowed vlan \<all/none/add/remove\> \<number\>  
(i) switchport trunk native vlan \<number\>  

\# sh int \<interface\>  
\# sh int trunk  

() int \<interface\>  
(i) speed \<10/100/auto\>  
(i) duplex \<full/half/auto\>  

(i) switchport port-security mac \<mac/sticky\>  
(i) switchport port-security maximum \<number\>  
(i) switchport port-security violation \<protect/restrict/shutdown\>  
(i) switchport port-security  
\# sh port-security  
\# sh port-security int \<interface\>  


() router rip  
  
