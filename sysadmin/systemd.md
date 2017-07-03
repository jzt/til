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
### Verify/lint unit

```
systemd-analyze verify my.service
```

### List jobs

```
systemctl list-jobs
```
