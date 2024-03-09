# Part 1
###    Cisco IOS (Internetwork Operating System) Family:
 - Cisco company Started With Routers
 -  IOS is Linux Based

#### CISCO OS types:

 - Cisco IOS
 - Cisco IOS XE
 - Cisco NX-OS
 - Cisco IOS XR

#### Other info:
         - POE ====> Power On Ethernet
  
         - PT Swiches are not real, they are packet tracer

         - 3650 Switches have modular Power


### Commands:

 | Command | Description |
 | --- | --- |
 | show version | it shows version of OS and more info |

 ---------------------------------------------------------------------

 
 # Part 2: 

 ### License:

 - Cisco Smart Software Manager (CSSM) ===> Sanctioans
 - Support for Permanent License Reservation (PLR)
 - Support for Specific Reservation (SLR)

### IOS Software Boot Sequence (Routers):

- step 1: POST
- step 2: copy the bootstrap program from ROM to RAM
- step 3: Bootstrap chooses the IOS image from Flash (Embeded or External) or Network (TFTP)
- Step 4: NVRAM Finds Start-up Config and Loads it

### IOS Modes:
- Main:
  - User EXEX Mode
  - Privileged EXEC Mode
  - Global Mode
- Other
  - ROM Monitor Mode
  - Setup Mode 

-----------------------------------------------------------------------------

# Part 3 & 4:

### Commands:

| Command | Description | Specifications | Sohrtened |
 | --- | --- | --- | --- |
 | ? | shows the commands | - | - |
 | enable | from user mode to privileged | - | en |
 | disable | Retuen to User mode | - | disa | 
 | configure terminal | from Privileged to Global Config | - | conf t |
 | eixt | From higher Mode to lower Mode | - | ex |
 | show | it shows sth | Only in Privileged Mode | - | 
 | brief | reduces the details of a command output| - | - |
 |show ip interface| info about ip interface | Privileged Mode | - |
 | ^z | from every higher Mode to Privileged Mode | other form: end | - |
 | ^R | Refresh: when your command is intrupted | - | - |
 | ^u | delete a line | - | - |
 | ^w| delete a word | - | - |
 | ^a | cursur goes to the beggining of a line | - | - |
 | ^shift6 | disable dns lookup | - | - |
 | hostname X | changes the device name | Global Mode| ho |
 | interface X | to go throught some physical interface | - | - |
 | no X | delete some config | - | - |
 | copy | :-) |  | privilieged |
 | reload | restart the system | | |
 | write memory | copy running-config stsrtup-config | Priviliged | wr|
 | do | run a privileged mode command in higher MOde| | |

restoring hostname to default: ```no hostname``` global mode

check stsrtup config ` show startup-config `

save the current config ` copy running-config stsrtup-config` Priviliged Mode OR `` write memory`` or `wr`


   #### Points:

        - Siwtches does'nt have NVRAM so they store the config in Flash storage
        - In Cisco you can type the command until you find them UNIQUE 
        - Most of the commands are writrn in Global Mode and the result will be cheked in Privileged Mode
        - startup config is what is kept in storage but running config lives in ram 
 
-----------------------------------------------------------------------------
