DD-Wrt commands
===============

#### Content 
1.[Web interface](#Web_interface)
2.[Wifi](#Wifi)
3.[Gathering info](#Gathering_info)

_________________
### Web interface
_________________

#### Start Web interface

```bash   
httpd -p 80
```

#### Stop Web interface
    killall httpd

#### Enable Web interface
    nvram set http_enable=1
    nvram commit

#### Disable Web interface
    nvram set http_enable=0
    nvram commit

____
### Wifi
____

#### Enable WiFi in N only mode
    nvram set ath0_net_mode=n2-only
    nvram commit

#### Disable WiFi
    nvram set ath0_net_mode=disabled
    nvram commit
 
__________________

### Gathering info
__________________

#### Show wireless devices
```bash
iw dev
```
#### Show connected wifi devices
    iw dev <interface> station dump

#### Show dhcp leases
    cat /tmp/dnsmasq.leases

#### Device names
    eth0 - Wan
    ath0 - WiFi (Atheros)
    br0  - Ehternet (192.168.1.1)
