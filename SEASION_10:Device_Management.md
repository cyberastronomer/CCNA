## Password Recovery:
- #### Routers:
    - POST ----> ^C ----> Rommon Mode -----> configuration registeration's
      - 0x2101: Boots into bootstrap, normal
      - 0x2142: Boots into ROM if initial boot fails
    - `confreg {reg mode}`
    - `boot`
    - `# dir flash`
    - `# copy startup-config running-config`
        - `(c) no user admin`
        - `(c) no enable secret`
    - Add User
    - Make enable pass
    - `(c) config-register 0x2102` ---> `do sh version` to check
- #### Switches:
    - Power off
    - Mode button 15s ---> Switch:
    - switch:
       - `flash_init`
    - `dir flash`
    - `rename flash:config.text flash:config.text.old`
    - `boot` ----> config not found
    - `copy flash:running-config`
       - config.text.old
          - name: running-config: enter (yes)
    - `no enable secret`
    - `no username {user}`
       - make a user
       - `(c-line) no login local`
    - `wr` OR `copy running-config startup-config `
    - `delete flash:config.text.old`
- #### Disable Password Recovery:
    - `(c) no service password-recovery`
- #### Securing Config and OS Image:
    - `# secure boot-image`
    - `# secure boot-config`
    - `# show secure bootset`
      
