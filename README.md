Sometimes, on older versions of Linux systems, an error appears when the touchpad does not work. Here are some tips to fix it.

### Open the GRUB default kernel boot parameters by typing
>sudo nano /etc/default/grub

### Then add the following line and save the file
>GRUB_CMDLINE_LINUX_DEFAULT="i8042.nopnp=1 pci=nocrs"

## Rebuild /boot/grub2/grub.cfg by adding the following line: 

>sudo grub2-mkconfig -o /boot/grub2/grub.cfg

Reboot your computer.

### You can also check which drivers are required for your touchpad. Usually, these are Synaptics and Elantech
>xinput list

### Once you have found out the model of your touchpad driver, you can try installing or reinstalling it


