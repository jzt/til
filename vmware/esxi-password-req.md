# Change ESXi Password complexity requirements

To remove password requirements edit `/etc/pam.d/passwd` and change `password requisite` line to:

```
password   requisite    /lib/security/$ISA/pam_passwdqc.so retry=3 min=1,1,1,1,1
```

### Resources

* https://kb.vmware.com/selfservice/microsites/search.do?language=en_US&cmd=displayKC&externalId=1012033
