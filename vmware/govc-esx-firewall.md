# govc ESX firewall

Disable ESX firewall with govc
```
govc host.esxcli network firewall set --enabled false
```

Show all firewall rules
```
govc host.esxcli network firewall ruleset list
```

Show all firewall rules detail
```
govc host.esxcli network firewall ruleset rule list
```

Show allowed IPs for all firewall rules
```
govc host.esxcli network firewall ruleset allowedip list
```
