# proxmox-setup
My simple Proxmox setup script for Dev Proxmox servers.

## Features ##

 - Disable Enterprise Repository
 - Enable "No subscription" Repository
 - Disable "Subscription Nag"
 - Update firmware to latest available
 - Install some extra useful commands
 - Enable IOMMU
 - Add some handy aliases
 - [PHPSYSINFO](https://phpsysinfo.github.io/phpsysinfo/) on port 80 (HTTP)

## Installation ##

From a `root` shell run the following command...

```
bash -c "$(wget -qLO - https://github.com/alandoyle/proxmox-setup/raw/main/proxmox-setup)"
```
