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
