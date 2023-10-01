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
 - [PHPSYSINFO](https://phpsysinfo.github.io/phpsysinfo/) on port 443 (HTTPS)
 - Add `setup-https` script.

## Installation ##

From a `root` shell run the following command...

```
bash -c "$(wget -qLO - https://github.com/alandoyle/proxmox-setup/raw/main/proxmox-setup)"
```
## setup-https

`setup-https` is a small script used to set up HTTPS on port 443.

It can detect and use custom SSL certs i.e. ACME certs (see https://pve.proxmox.com/wiki/Certificate_Management)

It can use the self-signed cert and key `/etc/pve/local/pve-ssl.pem` or an official cert `/etc/pve/local/pveproxy-ssl.pem`

The script is re-runnable and will automatically prefer an official certificate `/etc/pve/local/pveproxy-ssl.pem` thus allowing it to upgrade from a self-signed to a signed certificate easily.
