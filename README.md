Sometimes, on older versions of Linux systems, an error appears when the touchpad does not work. Here are some tips to fix it.
## Step 1 
sudo nano /etc/default/grub

GRUB_CMDLINE_LINUX_DEFAULT="i8042.nopnp=1 pci=nocrs"

## Step 2

sudo grub2-mkconfig -o /boot/grub2/grub.cfg
