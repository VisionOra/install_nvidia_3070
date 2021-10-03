# install_nvidia_3070 with ubuntu 18.04

Its the most difficult thing to install nvidia drivers that match with your nvidia version. I have 3070rtx and tried for almost 2 weeks to install nvidia drivers in ubuntu 18.06

<br>

## Steps

1. Install dependencies (gcc) https://linuxize.com/post/how-to-install-gcc-compiler-on-ubuntu-18-04/
2. Go to nvidia-offical site and download (https://www.nvidia.com/en-us/geforce/drivers/)
3. reboot
4. See if you system show blackscreen after ubuntu logo
5. If yes than press alt + ctrl + (f1 - f9) when ubuntu logo appear (you can see the error I am getting error of pysyical layer failure (power managment issue))
6. Force Restart the computer go to the grub and edit 
    a. GRUB_CMDLINE_LINUX_DEFAULT="quiet splash" to GRUB_CMDLINE_LINUX_DEFAULT="quiet splash pci=noaer"
7. Control x for restart
8. Hopefully you issue will be resolved
