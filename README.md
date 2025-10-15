```bash
pmbootstrap init
pmbootstrap install --no-split
pmbootstrap export
sudo losetup -P -f --show ~/.local/var/pmbootstrap/chroot_native/home/pmos/rootfs/generic-x86_64.img
sudo dd if=/dev/loopXXp1 of=/dev/____
```

```
search --no-floppy --fs-uuid --set=root <UUID>
linux	/boot/vmlinuz-stable psi=1 quiet  pmos_root_uuid=<UUID> pmos_rootfsopts=defaults
initrd	/boot/amd-ucode.img
initrd	/boot/intel-ucode.img
initrd	/boot/initramfs

```
