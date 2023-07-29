# Proxmox-Script
Proxmox-Script

Available now: Create VM Template from Cloud-Image and Cloud-Init

## How to use ?

Clone this repo and copy file to your PATH (**/usr/local/bin** or other path) and give execution permissions **chmod +x**

Download Cloud-Image-File

* Debian [https://cloud.debian.org/images/cloud/](https://cloud.debian.org/images/cloud/)
* Ubuntu [https://cloud-images.ubuntu.com/](https://cloud-images.ubuntu.com/)
* Centos [https://cloud.centos.org/](https://cloud.centos.org/)
* AlmaLinux [https://wiki.almalinux.org/cloud/Generic-cloud.html](https://wiki.almalinux.org/cloud/Generic-cloud.html)

Run The Command:

```
create-template vmid name cpu ram net disk image-file
```

For using cloud-init in Proxmox, you can read here:

* [https://pve.proxmox.com/wiki/Cloud-Init_Support](https://pve.proxmox.com/wiki/Cloud-Init_Support)
