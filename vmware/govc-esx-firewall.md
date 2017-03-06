# govc ESX firewall

Disable ESX firewall with govc
```
govc host.esxcli network firewall set --enabled false
```

Show all firewall rules by name and their status
```
govc host.esxcli network firewall ruleset list
```

Show all firewall rules by name with port and protocol detail
```
govc host.esxcli network firewall ruleset rule list
```

Show single firewall rule by name with port and protocol detail
```
govc host.esxcli network firewall ruleset rule list --ruleset-id=<ID>
```

Show allowed IPs for all firewall rules
```
govc host.esxcli network firewall ruleset allowedip list
```
