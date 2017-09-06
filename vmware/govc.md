# govc

### Get vCenter hostname

```
govc option.ls config.vpxd.hostnameUrl
govc option.ls config.vpxd.instanceName
```

### Dump VM info

```
govc vm.info -json vm_name | jq '.' | cat > outfile
```
