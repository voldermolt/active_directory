# Active Directory 

## Installing VMs
1. Download the needed isos 
    - Windows 2016 server
    - Windows 10 
2. Install VMware player 
3. When Installing the 2016 server add the iso file at the end.


# Installing the Domain Controller

1. Use `sconfig` to:
    - Change the hostname
    - Change the IP address to static
    - Change the DNS server to our own IP address
2. Install the Active Directory Windows Feature 

```shell
Install-WindowsFeature AD-Domain-Services -IncludeManagementTools
```