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

### Get VM moid

```
govc vm.info -dump -json vm_name | jq -c '.VirtualMachines[] | .Self.Value'
```
