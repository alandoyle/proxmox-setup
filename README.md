# proxmox-setup
My simple Proxmox setup script

## Features ##

 - Disable Enterprise Repository
 - Enable "No subscription" Repository
 - Disable "Subscription Nag"
 - Add Edge Kernel
 - Update firmware to latest available
 - Install some extra useful commands
 - Enable IOMMU
 - Add some handy aliases
 
## Installation ##

From a `root` shell run the following command...

```
bash -c "$(wget -qLO - https://github.com/alandoyle/proxmox-setup/raw/main/proxmox-setup)"
```
