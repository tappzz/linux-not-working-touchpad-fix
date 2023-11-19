Some fixes
sudo nano /etc/default/grub
GRUB_CMDLINE_LINUX_DEFAULT="i8042.nopnp=1 pci=nocrs"
sudo grub2-mkconfig -o /boot/grub2/grub.cfg
