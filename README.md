<img width="1920" height="1080" alt="Снимок экрана от 2025-09-30 17-33-01" src="https://github.com/user-attachments/assets/5ba94369-57ff-4e7b-a819-3ef33984aa02" />



# Installation

> ### __The theme only supports 1080р__

1. #### Clone the repository or download the archive

```
# git clone https://github.com/Sameguyy/2B-grub2-theme.git
```

2. #### Copy the theme folder to the GRUB directory

```
# sudo mkdir -p /boot/grub/themes
```
 
```
# sudo cp -r 2B-grub2-theme /boot/grub/themes/
```

3. #### Open GRUB config
```
# sudo nano /etc/default/grub
```
   
   Find the following lines and set the values:
   
   ``GRUB_TERMINAL_OUTPUT="gfxterm"`` #turns on graphics mode in grub
   
   ``GRUB_GFXMODE=1920х1080`` #resolution
   
   ``GRUB_THEME="/boot/grub/themes/2B-grub2-theme/theme.txt"`` #path to /theme.txt

4. #### Update GRUB
Arch / Manjaro / EndeavourOS
```
# grub-mkconfig -o /boot/grub/grub.cfg
```

   Fedora / RHEL / CentOS
    
```
# grub2-mkconfig -o "$(readlink -e /etc/grub2.conf)"
```

   Ubuntu / Debian / etc..
```
# update-grub
```
