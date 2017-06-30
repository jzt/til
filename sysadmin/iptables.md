# iptables

### Show all rules

```
iptables --list-rules <chain>
```

Options:
* list-rules - Print all rules (in chain)

### Show all rules 

```
iptables -L -n -v
```

Options:
* n - show numeric port numbers
* v - verbose

### Allow ping

```
iptables -A INPUT -p icmp --icmp-type echo-request -j ACCEPT
iptables -A OUTPUT -p icmp --icmp-type echo-reply -j ACCEPT
```

### Allow SSH

```
iptables -A INPUT -p tcp --dport 22 -m state --state NEW,ESTABLISHED -j ACCEPT
iptables -A OUTPUT -p tcp --sport 22 -m state --state ESTABLISHED -j ACCEPT
```
