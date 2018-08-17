# Networking

### Static IP with Systemd

`/etc/systemd/network/eth0.network`

```
[Match]
Name=eth0
[Network]
Address=192.168.100.2/24
Gateway=192.168.100.1
DNS=192.168.100.1
```

```
systemctl enable systemd-networkd.service
systemctl enable systemd-resolved.service
```

### Show routes
```
ip route show
```

macOS
```
netstat -nr
```
