# iptables

### Show all rules

```
iptables --list-rules _chain_
```

Options:
* list-rules - Print all rules (in chain)


### Allow ping

```
iptables -A INPUT -p icmp --icmp-type echo-request -j ACCEPT
iptables -A OUTPUT -p icmp --icmp-type echo-reply -j ACCEPT
```
