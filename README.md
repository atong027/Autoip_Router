# Auto Change IP v2

## Supported Router

✔ mipsel_24kc

❌ mips_24kc [wait nyo lang]

## Installation

- download package [here](https://github.com/atong027/Autoip_Router/releases)
  - extract po
  - login po sa router [webui](http://192.168.1.1/cgi-bin/luci/)
  - punta po dito sa [software](http://192.168.1.1/cgi-bin/luci/admin/system/opkg)
  - click po yung update list ( wait matapos )
  - upload package --> then iupload yung file na .ipk
  - tapos install


- using putty/cmd
  - open putty/cmd
  - login sa ssh router
  - copy paste itong command 
    
    `curl -o /tmp/autoip.tar.gz -L https://github.com/atong027/Autoip_Router/files/5470874/autoip.tar.gz`
  
    `tar xzf /tmp/*.gz -C /tmp/ && opkg update && opkg install /tmp/*.ipk`

## How to run

- send lang po sa ssh (putty/cmd) `autoip` para sa mga commands

  `autoip start`                  - start script
  
  `autoip stop`                   - stop script
  
  `autoip details`                - set modem information **(NOTE: eto po need irun after ma install)**
  
  `autoip status`                 - logs
  
  `logread -fe autoip`            - live logs
  
  `/etc/init.d/autoip enable`     - enable sa startup
  
  `/etc/init.d/autoip disable`    - disable sa startup
  
## NOTE

- Need palitan apn to globe prepaid apn if hindi nag chachange ip after mag turn off on data
- Need ko copy [mac address](https://m.me/ayrton.ilagan) ng modem para ma add ko kayo sa list **💲💲💲**

## TO DO

- [ ] Add ibang router
- [ ] Add video instruction or pictures (baka naman meron dyan gumawa 😂)

## BUGS

- if ayaw po mag start kahit na nilagay nyo `autoip stop` tapos `autoip start`
  eto po fix `rm /var/run/autoip.pid` tapos start nyo na `autoip start`
  
   
   
