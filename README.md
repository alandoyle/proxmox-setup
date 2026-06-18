# proxmox-setup
My simple Proxmox setup script for Dev Proxmox servers.

## Special note

This script can be safely run on PVE v9.x/PBS 4.x with a valid subscription as long as it's configured to do so before being run.

To use this script with a subscription run the following command before installing he script.

```
echo "PROXMOX_ENV=LIVE" > /etc/default/proxmox-setup
```

## Features ##

 - Supports Proxmox 8.2 or higher
 - Supports Proxmox Backup Server 3.2 or higher
 - Disable Enterprise Repository
 - Enable "No subscription" Repository
 - Disable "Subscription Nag"
 - Update firmware to latest available
 - Enable IOMMU

### Full Installation Additional Features

 - Install some extra useful commands
 - Add some handy aliases
 - Setup Log2RAM and configure journald
 - Tweak system settings for better performance.

## Installation ##

From a `root` shell run one of the following commands...

### Full PVE v9.x/PBS v4.x Installation

```
bash -c "$(wget -qLO - https://github.com/alandoyle/proxmox-setup/raw/main/proxmox-setup)"
```

### Minimal PVE v9.x/PBS v4.x Installation

```
bash -c "$(wget -qLO - https://github.com/alandoyle/proxmox-setup/raw/main/proxmox-minimal-setup)"
```

### Upgrade from Proxmox 8.x 'Bookworm' to 9.x 'Trixie'

```
bash -c "$(wget -qLO - https://github.com/alandoyle/proxmox-setup/raw/main/upgrade-proxmox)"
```

### Full PVE v8.x/PBS v3.x Installation

```
bash -c "$(wget -qLO - https://github.com/alandoyle/proxmox-setup/raw/main/proxmox-setup-v8)"
```

### Minimal PVE v8.x/PBS v3.x Installation

```
bash -c "$(wget -qLO - https://github.com/alandoyle/proxmox-setup/raw/main/proxmox-minimal-setup-v8)"
```
