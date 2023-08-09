# Proxmox-Script
Proxmox-Script

Available now: Create VM Template from Cloud-Image and Cloud-Init

## How to use ?

Run on Proxmox Console/SSH Server

Clone this repo and copy file to your PATH (**/usr/local/bin** or other path) and give execution permissions **chmod +x**

Download Cloud-Image-File

* Debian [https://cloud.debian.org/images/cloud/](https://cloud.debian.org/images/cloud/)
* Ubuntu [https://cloud-images.ubuntu.com/](https://cloud-images.ubuntu.com/)
* Centos [https://cloud.centos.org/](https://cloud.centos.org/)
* AlmaLinux [https://wiki.almalinux.org/cloud/Generic-cloud.html](https://wiki.almalinux.org/cloud/Generic-cloud.html)

Run The Command:

```
create-template vmid name cpu memory net disk image-file
```


After that run script *create-vm* 

```
create-vm 101 1001 vm-ubuntu
```

For using cloud-init in Proxmox, you can read here:

* [https://pve.proxmox.com/wiki/Cloud-Init_Support](https://pve.proxmox.com/wiki/Cloud-Init_Support)
