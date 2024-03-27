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
  
      
