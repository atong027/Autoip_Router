# Auto Change IP

## Supported Router

✔ mipsel_24kc

❌ mips_24kc [wait nyo lang]

## Installation

- download package [here](https://github.com/atong027/Autoip_Router/files/5470874/autoip.tar.gz)
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
  - eto pa `tar xzf /tmp/*.ipk -C /tmp/ && opkg update && opkg install /tmp/*.ipk`

# Hindi pa tapos
