# tcpdump

### Capture DHCP

```
sudo tcpdump -i <network-interface> port 67 or port 68 -e -n -w capture.pcap
```

### Capture IP range

```
sudo tcpdump -n dst net 10.0.0.0/8 -w capture.pcap
```
