# LAST UPDATE THIS YEAR [2020] (12/19/20)

# Auto Change IP v2

## Supported Router

✔ mipsel_24kc

❌ mips_24kc [wait nyo lang]

## Installation

- download package [here](https://github.com/atong027/Autoip_Router/releases)
  - login po sa router [webui](http://192.168.1.1/cgi-bin/luci/)
  - punta po dito sa [software](http://192.168.1.1/cgi-bin/luci/admin/system/opkg)
  - click po yung update list ( wait matapos )
  - upload package --> then iupload yung file na .ipk
  - tapos install

## How to run

- send lang po sa ssh (putty/cmd) `autoip` para sa mga commands

  `autoip start`                  - start script
  
  `autoip stop`                   - stop script
  
  `autoip details`                - set modem information **(NOTE: eto po need irun after ma install)**
  
  `autoip status`                 - logs
  
  `/etc/init.d/autoip enable`     - enable sa startup
  
  `/etc/init.d/autoip disable`    - disable sa startup
  
## NOTE

- ~~Need palitan apn to globe prepaid apn if hindi nag chachange ip after mag turn off on data~~
- Need ko copy [mac address](https://m.me/ayrton.ilagan) ng modem para ma add ko kayo sa list **💲💲💲**

## TO DO

- [ ] Add ibang router
- [ ] Add video instruction or pictures

## BUGS

- ~~if ayaw po mag start kahit na nilagay nyo `autoip stop` tapos `autoip start`~~

  ~~eto po fix `rm /var/run/autoip.pid` tapos start nyo na `autoip start`~~
  
   
   
