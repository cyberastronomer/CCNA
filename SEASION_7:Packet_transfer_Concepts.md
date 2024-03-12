# Part 1,2,3:

#### Hub wicknesses:
- collision
- Broadcast
- security

#### APIPA:
```When a Windows computer isn't able to communicate with the DHCP server, something called Automatic Private IP Addressing (APIPA) kicks in. It assigns the computer an IP address that starts with 169.254. These IP addresses are only useful on local networks, not the internet```

------------------------------------------------------------
#### ARP:
![alt text](https://yurmagccie.files.wordpress.com/2018/04/arp-draw_io.jpg)

- ##### Points:
    - Cisco switches stores the new mac address of each interface in some plcae called ``` mac address table ``` which is visible by ```show mac-address-table```
    - Windows devices also store the new mac addresses, visible by ``` arp -a ```
    - Arp ping ===> layer 2, passing firewall  in order to check if it's blocking the ip or not
    - Updating Mac Address ===> GARP: announcing new mac address using ARP ===> Update Arp Table: used by hackers
    - New IP ===> Announcd by ARP: 1- No reply ===> Change 2- reply ===> IP forbidden 3- off PC ===> Dup IP
    - cleared ARP-Table Switch: switch foolding after an L2 packet: all interfce Boradcast
-----------------------------------------------------------------

## Senario:
![senario](./pic/s0.png)
