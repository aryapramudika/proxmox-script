# Proxmox-Script
Proxmox-Script (PSH)

* Create Template from Cloud Images
* Create VM Based On Template
* Delete VM used VM Name

## How to use ?

Run on Proxmox Console/SSH Server

Clone this repo and copy file to your PATH (**/usr/local/bin** or other path) and give execution permissions **chmod +x**

```bash
cp proxmox-script/psh /usr/local/bin && chmod +x /usr/local/bin/psh
```

Download Cloud-Image-File

* Debian [https://cloud.debian.org/images/cloud/](https://cloud.debian.org/images/cloud/)
* Ubuntu [https://cloud-images.ubuntu.com/](https://cloud-images.ubuntu.com/)
* Centos [https://cloud.centos.org/](https://cloud.centos.org/)
* AlmaLinux [https://wiki.almalinux.org/cloud/Generic-cloud.html](https://wiki.almalinux.org/cloud/Generic-cloud.html)

Run This Script:

```bash
psh
Usage: /usr/local/bin/psh <createvm/createtemplate/deletevm>
```

Create Template

```bash
psh createtemplate
Usage: /usr/local/bin/psh createtemplate <vmid> <name> <cpu> <memory> <net> <disk> <image-file>
Example: /usr/local/bin/psh createtemplate 1001 template-ubuntu-20 2 4096 vmbr0 local-lvm focal-ubuntu.img
```

Create VM

```bash
psh createvm
Usage: /usr/local/bin/psh createvm <template-id> <vmid> <name> <cpu> <memory> <disk>
Example: /usr/local/bin/psh createvm 901 101 debian-vm 4 4 30G
```

Delete VM

```bash
psh deletevm
Usage: /usr/local/bin/psh deletevm <name>
Example: /usr/local/bin/psh deletevm debian-vm
```
Details about how to use cloud-init in Proxmox, you can read in here:

* [https://pve.proxmox.com/wiki/Cloud-Init_Support](https://pve.proxmox.com/wiki/Cloud-Init_Support)
