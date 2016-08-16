# Install ESX UI (Embedded Host Client)

1. [Download VIB](http://download3.vmware.com/software/vmw-tools/esxui/esxui-signed-4215448.vib)
2. `scp esxui-signed-4215448.vib root@<esxip>:/tmp`
3. `ssh root@<esxip> esxcli software vib install -v /tmp/esxui-signed-4215448.vib`

### Resources

* https://labs.vmware.com/flings/esxi-embedded-host-client
