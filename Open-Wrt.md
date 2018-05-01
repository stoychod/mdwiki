#### Start Web interface
    /etc/init.d/uhttpd start

#### Stop Web interface
    /etc/init.d/uhttpd stop

#### Enable Web interface at boot
    /etc/init.d/uhttpd enable

#### Show wireless devices
    iw dev

#### Show connected wifi devices
    iw dev <interface> station dump

#### Show dhcp leases
    cat /tmp/dhcp.leases

#### Append ssh_pub keys to authorised_keys file
Example:
    
    ssh root@192.168.1.1 "/bin/cat >> /etc/dropbear/authorized_keys " < stoycho@SM-N9005_rsa.pub
