```bash
pmbootstrap init
pmbootstrap install --single-partition
pmbootstrap export
sudo dd if=~/.local/var/pmbootstrap/chroot_native/home/pmos/rootfs/generic-x86_64.img of=/dev/____
```

```
search --no-floppy --fs-uuid --set=root <UUID>
linux	/boot/vmlinuz-stable psi=1 quiet  pmos_root_uuid=<UUID> pmos_rootfsopts=defaults
initrd	/boot/amd-ucode.img
initrd	/boot/intel-ucode.img
initrd	/boot/initramfs
```
