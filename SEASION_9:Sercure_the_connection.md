# Sercuring the connection:
 - choosing the console line: ` (c) line console 0 `
 - set password `password {pass}`
 - enable the login process: `(c-line) login ` opposite: `no login`
 - to see the users: `(#) show user`
 - hiding the password in config by hash & salt: `(c) service password-encyption` opposite : `no " " "`
 - to see the config based on console lines: `(#) show run | begin line`
 - ####  Adding User:
    - `username admin password {pass}`
    - enabling authentication for each line : `(c-line) login local `


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
