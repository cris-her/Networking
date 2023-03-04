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

sw() int \<interface\>  
sw(i) switchport mode trunk  
rtr() int \<interface\>  
rtr(i) no ip ad  
rtr(i) no sh  
rtr(i) ex  
rtr() int \<interface\>.\<number\>  
rtr(si) encapsulation dot1q \<number\>  
rtr(si) ip add \<ip\> \<mask\>  
rtr(si) description \<description\>  

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
(r) no auto-summary  
\# debug ip rip  
\# undebug all  
\# sh ip protocols  

() router ospf \<process \#\>  
(r) network \<network id\> \<wcm\> area \<\#\>  
\# show ip protocols  
\# show ip ospf  
\# show ip ospf interface  
\# show ip ospf neighbor  
\# show ip ospf database  

() router eigrp \<\#\>  
(r) network \<network id\> \<inverted mask\>  
\# sh run  
\# sh ip protocols  
\# sh ip eigrp interface  
\# show ip eigrp neighbor  
\# show ip eigrp topology  

--> cisco hdlc config  
The default encapsulation for Serial Link  
Only need to Enable the link and configura IP Address  

ipconfig  
() int g0/0  
(i) ipv6 address 2001:120:1:1::1/64  
(i) ipv address FE80::1 link-local  
(i) ipv address 2010::/64 eui-64  
(i) no sh  
\# sh ipv int bri  
\# sh ipv route  
\# sh ipv int g0/0  
\# ping FE80::290:2BFF:FE52:6901  
gi0/0  

() ipv route 2001:11::0/64 2001:120:1:1::1 ?  
() ipv unicast routing  

() int \<interface\>  
(i) ipv6 rip \<name\> enable  

() int \<interface\>  
(i) ip add \<ip\> \<mask\>  
(i) no sh  
() ip dhcp pool \<name\>  
(d) default-router \<gateway ip\>  
(d) network \<network\> \<mask\>  
(d) dns-server \<dns ip\>  
() ip dhcp excluded-address \<from ip\> \<to ip\>  

--> dhcp relay server  
() int \<interface\>  
(i) ip helper-address \<dhcp server ip\>  

--> classic syntax  
() access-list \<ACL_No\> \<deny/permit\> \<matching parameters\>  
--> extended  
() access-list \<ACL_No\> \<deny/permit\> \<Protocol\> \<Source IP\> \<Wildcard Mask\> [Protocol Info] \<Destination IP\> \<Wildcard Mask\> [Protocol Info]  

--> modern syntax  
() ip access-list standart \<ACL_No./Name\>  
(s) \<deny/permit\> \<matching parameters\>  
--> extended  
() ip access-list extended \<ACL_No./Name\>  
(e) \<deny/permit\> \<Protocol\> \<Source IP\> \<Wildcard Mask\> [Protocol Info] \<Destination IP\> \<Wildcard Mask\> [Protocol Info]  

--> apply the ACL  
() int \<type & slot\#\>  
(i) ip access-group \<ACL_No./Name\> \<in/out\>  
