# Using VIBs

### Install

* Check current acceptance level: `esxcli software acceptance get`
* If VIB needs community supported, set acceptance level: `esxcli software acceptance set --level CommunitySupported`
* `scp vic-firewall.vib root@<esxip>:/tmp`
* `ssh root@<esxip> esxcli software vib install -v /tmp/vic-firewall.vib`
* Check that the VIB is installed: `esxcli software vib list` or `esxcli software vib get -n
  vic-firewall`

### Remove

* Remove VIB: `esxcli software vib remove --vibname vic-firewall`

### Build a VIB

* TODO

### Resources

* https://pubs.vmware.com/vsphere-55/index.jsp?topic=%2Fcom.vmware.vsphere.security.doc%2FGUID-751034F3-5337-4DB2-8272-8DAC0980EACA.html
