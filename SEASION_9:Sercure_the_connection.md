```cisco
enable
!
conf t
!
username admin secret 123456
!
line console 0
  login local
  no exec-timeout
  end
!
exit 
```
telnet config
```cisco

en
conf t
!
hostname r1
!
int g 0/0/0
  no sh
  ip add 192.168.1.1 255.255.255.0
  exit
!
int g 0/0/1
  no sh
  ip add 192.168.2.1 255.255.255.0
  exit
!
line console 0
  login local
  exit
!
username admax secret 123456
!
enable secret 321
end
!
wr
```
