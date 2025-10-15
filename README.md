```bash
pmbootstrap init
pmbootstrap install --no-split
pmbootstrap export
sudo losetup -P -f --show ~/.local/var/pmbootstrap/chroot_native/home/pmos/rootfs/generic-x86_64.img
sudo dd if=/dev/loopXXp1 of=/dev/____
```
