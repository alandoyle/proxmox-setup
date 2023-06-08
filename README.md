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
 - Add `setup-https-redirect` script.

## Installation ##

From a `root` shell run the following command...

```
bash -c "$(wget -qLO - https://github.com/alandoyle/proxmox-setup/raw/main/proxmox-setup)"
```
## setup-https-redirect

`setup-https-redirect` is a small script used to set up a redirect from port 443 to 8006.

It can detect and use custom SSL certs i.e. ACME certs (see https://pve.proxmox.com/wiki/Certificate_Management)

It can use the self-signed cert and key `/etc/pve/local/pve-ssl.pem` or an official cert `/etc/pve/local/pveproxy-ssl.pem`

The script is re-runnable and will automatically prefer `/etc/pve/local/pveproxy-ssl.pem` thus allowing it to upgrade the redirect from self-signed to signed certificate easily.
