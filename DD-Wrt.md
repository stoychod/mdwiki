DD-Wrt commands
===============

#### Content
1. [Web interface](#web-interface)
2. [Wifi](#wifi)
3. [Gathering info](#gathering-info)

<br><br>

## Web interface
_________________

#### Start Web interface

```bash   
httpd -p 80
```

#### Stop Web interface
    
```bash
killall httpd
```

#### Enable Web interface
    
```bash    
nvram set http_enable=1
nvram commit
```

#### Disable Web interface
    
```bash
nvram set http_enable=0
nvram commit
```

<br><br>

## Wifi
____

#### Enable WiFi in N only mode
    
```bash    
nvram set ath0_net_mode=n2-only
nvram commit
```

#### Disable WiFi
    
```bash
nvram set ath0_net_mode=disabled
nvram commit
``` 
<br><br>

## Gathering info
__________________

#### Show wireless devices

```bash
iw dev
```

#### Show connected wifi devices
    
 ```bash   
iw dev <interface> station dump
```

#### Show dhcp leases
    
```bash    
cat /tmp/dnsmasq.leases
```

#### Device names

```    
eth0 - Wan
ath0 - WiFi (Atheros)
br0  - Ehternet (192.168.1.1)
```
