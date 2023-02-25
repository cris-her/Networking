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
() banner motd \<char\>  
\<message\> \<char\>  
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
() int \<interface\>  
() int range f0/2-3  
(i) switchport mode access  
(i) switchport access vlan \<number\>  

() vtp pruning  
() int gi0/1  
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

() hostname \<name\>  
() line con 0  
(l) password \<password\>  
(l) login  
() service password-encryption  
--> cisco encryption 7 decoder  
() enable secret \<password\>  
() line vty 0 4  
(l) password \<password\>  
(l) login  
() int \<interface\>  
(i) ip address \<ip\> \<mask\>  
(i) no sh  
() banner motd \<char\>  
\<message\> \<char\>  
\# copy running-config startup-config  
\# sh startup-config  
\# sh ip route  
\# sh ip int \<interface\>  

() ip route \<network id\> \<mask\> \<next hop/exit interface\>  
() no ip route \<network id\> \<mask\> \<next hop/exit interface\>  

() router rip  
(r) ver 2  
(r) network \<network id\>  

sw() int \<interface\>  
sw(i) switchport mode trunk  
rtr() int \<interface\>  
rtr(i) no ip ad  
rtr(i) no sh  
rtr(i) ex  
rtr() int \<interface\>.\<number\>  
rtr(si) encapsulation dot1q vlan \<number\>  
rtr(si) ip add \<ip\> \<mask\>  
rtr(si) description \<description\>  

