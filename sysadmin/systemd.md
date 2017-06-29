# systemd

### List all failed units 

```
systemctl list-units --state=failed
```

### List dependencies

Show dependencies (units required or wanted) to start the named unit. 

```
systemctl list-dependencies sshd.service
```
