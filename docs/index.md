# Core Linux 

Core Linux is a new distribution based on Arch Linux, developed by the Italian community Architalia. It is described as a friendly, powerful, and easy-to-use distribution. Its installation is done through a configuration script that guides the user in choosing the system configuration options.

![image](https://github.com/ArchItalia/core/assets/117321045/0a0ee32c-d329-4570-a2e3-5bf843a6be70)




![image](https://github.com/ArchItalia/core/assets/117321045/fd0f00cb-0225-4572-bcf3-ac701545518f)


## Installation

The script starts by asking for the language to use during installation and shows a brief description of the project and the community that develops it. Then, it enters a series of guided choices to configure the system, starting with the selection of language, time zone, and character map.

![image](https://github.com/ArchItalia/core/assets/117321045/96c5364b-0aca-4e23-b6ac-a5add14dcbc2)


The process continues with the choice of the username, which is used to create the user account, the user password, and the root password encrypted with a securely generated key. The user can also choose one of the three available shells: bash, zsh, or fish.

Next, the user is guided to choose among four possible AUR helpers and four possible firewalls: firewalld, ufw, iptables, or none. In addition, it's possible to choose the standard linux kernel or other versions such as linux-lts, linux-zen, linux-hardened, each with different features.

Once some choices are made about which packages to install and which base version to select, the configuration of the disk partition is reached, where it is possible to choose the device on which to install the operating system, the file system format, and the partition size.

The installation continues with the choice of the swap partition size. Then it's asked to select the nearest server mirror, and finally, an overview of all the choices made is presented. Here the user can choose to confirm and proceed with the installation or go back to the configuration phase to make changes.

Finally, the script starts the actual installation, using the configuration file created earlier. The system installation will take some time depending on the power of the user's computer and the number of selected packages.

In summary, Core Linux is an Arch Linux-based distribution designed to be friendly, powerful, and easy to use. The installation script provides a guided and simplified experience, allowing the user to customize their system securely and quickly.

![image](https://github.com/ArchItalia/core/assets/117321045/2c32b29f-8da9-480e-9efb-b0e8b4c0186e)


## System Clean 

Clean is a tool created by the Core Linux team developers for system maintenance to remove orphan packages, package cache, user cache, and trash. Just type the `clean` command or use the application in the menu.

![image](https://github.com/ArchItalia/core/assets/117321045/96ad1dfc-09e7-45f0-bdfd-43eca52feee3)


## Downgrade packages


Downgrade is a tool for package storage in Arch Linux that allows users to revert to a previous version of a package. Arch Linux users can use Downgrade when system updates cause issues with the latest version of an installed package. For example, a new feature may have been added that the user does not like, or there may be bugs that prevent the use of the package.

![image](https://github.com/ArchItalia/core/assets/117321045/6840e6ac-22b4-4ee5-ab4c-291ba40cd78c)


To use Downgrade, the user must connect to the Core Linux console as a root user and launch the command 'downgrade package name'. The program displays a list of all installed packages in chronological order, from newest to oldest. The user can select the package they want to revert and choose the previous version they want to downgrade to. It should be noted that users can use a previous version of a package that is either installed in the package cache or remotely.

## Timeshift

With the help of TimeShift, users can take a snapshot of the system before performing a major update or installing new software packages. In case of any issues during the update, using TimeShift allows for easy restoration of the previous system state without any loss of data or customized configurations.


![image](https://github.com/ArchItalia/core/assets/117321045/fc364aaf-34ef-4c89-9cc0-8e4688eec6d0)



## Version Minimal and Full

The main difference between the Minimal and Full versions of Core Linux is related to the packages included in the basic installation. The Minimal version includes only the essential packages necessary to make the operating system work, such as the Arch Linux base core, libraries, fonts, themes, the Xorg graphical client, the GNOME desktop environment with some accessories like Nautilus, the network manager, the CUPS printing utility, and other utility packages like cronie and Git.

In the Full version, instead, we also find packages like LibreOffice (an open-source alternative to Microsoft Office), Blender and Inkscape (3D graphics and animation programs), GIMP (a powerful image editor), VLC (a media player), and many other useful tools such as advanced text editors, productivity programs, applications for contact management, system utilities, communication applications, and many others.

For both versions, the user can choose the type of AUR helper, firewall, and shell to use. Also, the installation requires the user to select a mirror server and the kernel version to use.

In general, the Minimal version is designed to provide a solid foundation for building a customized operating system, while the Full version is more complete and offers many ready-to-use features for the average user. However, with both versions, the user has the flexibility to further customize their system according to their needs and preferences.

Base packages in the Minimal Version:

```
* papirus-icon-theme
* papirus-nord
* color-folders
* clean
* nautilus
* cups
* cronie
* git
* wget
* reflector
* bluez
* bluez-utils
* gnome-shell-extension-desktop-icons-ng
* firefox
* downgrade
* timeshift
* extension-manager
* evince
* eog
* gparted
* gsmartcontrol
* mpv
* gnome-calculator
* gnome-clocks
* gnome-calendar
* gnome-terminal
* gnome-text-editor
* htop
* gnome-system-monitor
* vim
* nano
* neofetch
* liferea 
```

Additional packages in the Full version:
```
* etcher-bin
* gnome-font-viewer
* libreoffice
* vlc
* blender
* inkscape
* gimp
* gnome-weather
* gnome-maps
* gnome-contacts
* gnome-disk-utility
* thunderbird
* transmission-gtk
* remmina
* cheese
* rhythmbox
* simple-scan
* telegram-desktop
* obs-studio
* discord
* lutris
* code
* gnome-boxes
* foliate
* darktable
```

User-selectable options:
```
(aur helpers) yay, paru, aura, pikaur. 
(firewall) firewalld, ufw, iptables.
(shell) zsh, fish
```
<br>

## Color-folders

With color-folders, you can change the style of your Papirus icons among 45 different themes.

![image](https://github.com/ArchItalia/core/assets/117321045/b4206086-66c4-4388-8cb5-b61652d9b9b6)

![Screenshot from 2023-08-07 16-12-09](https://github.com/ArchItalia/core/assets/117321045/6de8658f-2147-4686-a4d7-8937c60e80fc)


<br>

## Nvidia Support

![image](https://github.com/ArchItalia/core/assets/117321045/9c82c096-89c7-4ee9-99c6-5ef9c9b89315)

Base support for nvidia driver installation and Nvidia Optimus configuration for gdm display manager.

Install nvidia packages:

```
sudo pacman -S nvidia nvidia-utils nvidia-settings libva-utils libva-vdpau-driver libva-mesa-driver
```

Create the hooks directory and add the configuration:

- `sudo mkdir -p /etc/pacman.d/hooks`
- `sudo vim /etc/pacman.d/hooks/nvidia.hook`

```
[Trigger]
Operation=Install
Operation=Upgrade
Operation=Remove
Type=Package
Target=nvidia


[Action]
Description=Update Nvidia module in initcpio
Depends=mkinitcpio
When=PostTransaction
Exec=/usr/bin/mkinitcpio -P

```

Create the nouveau blacklist file as root:

`sudo vim /etc/X11/xorg.conf.d/10-nvidia-drm-outputclass.conf`

```
Section "OutputClass"
Identifier "intel"
MatchDriver "i915"
Driver "modesetting"
EndSection

Section "OutputClass"
Identifier "nvidia"
MatchDriver "nvidia-drm"
Driver "nvidia"
Option "AllowEmptyInitialConfiguration"
Option "PrimaryGPU" "yes"
ModulePath "/usr/lib/nvidia/xorg"
ModulePath "/usr/lib/xorg/modules"
EndSection

```

Display Manager Configuration for GDM

`sudo vim /usr/share/gdm/greeter/autostart/optimus.desktop`

```
[Desktop Entry]
Type=Application
Name=Optimus
Exec=sh -c "xrandr --setprovideroutputsource modesetting NVIDIA-0; xrandr --auto"
NoDisplay=true
X-GNOME-Autostart-Phase=DisplayServer

```

`sudo vim /etc/xdg/autostart/optimus.desktop`

```
[Desktop Entry]
Type=Application
Name=Optimus
Exec=sh -c "xrandr --setprovideroutputsource modesetting NVIDIA-0; xrandr --auto"
NoDisplay=true
X-GNOME-Autostart-Phase=DisplayServer

```

Mkinitcpio

Edit the mkinitcpio.conf file and add the following to our configuration and add kernel modules:

`sudo vim /etc/mkinitcpio.conf`

```
MODULES=(btrfs nvidia nvidia_modeset nvidia_uvm nvidia_drm)

```

`sudo mkinitcpio -P`


Xinitrc

Add to the .xinitrc file or create it if it does not exist in `~/.xinitrc`

```
xrandr --output <output-name> --set "PRIME Synchronization" 1
```

Finally, add the kernel parameter `nvidia_drm.modeset=1 ` in your bootloader configuration:

GRUB:

```
GRUB_CMDLINE_LINUX="nvidia-drm.modeset=1"
```

`# grub-mkconfig -o /boot/grub/grub.cfg`

Systemd-boot:

For example, if your configuration is in `/boot/loader/entries/arch.conf`

```
options root=/dev/xxx  rootflags=subvol=@ rw quiet loglevel=3 rd.system.show_status=auto rd.udev.log_level=3 nvidia-drm.modeset=1

```

Restart the machine `$ reboot`

<br> 

## Download 

[Download Core-2023.08.16-x86_64.zip](https://drive.google.com/file/d/1wYXX8MAlWTeN_KYtivc-wYczJxqqZY2U/view?usp=sharing) 

`sha256sum 65e79b06f981f9c65d4867377d8599407c5ca95b148e4df46756cab30f07d67c  Core-2023.08.16-x86_64.iso`

!!! warning
   
    requires the entire disk to be used during installation.

!!! info

    - Core Linux
    - installcore v.2.1
    - version 2023.8 Beta
    - size 1.48G
    

NOTE: Pacman will complain about importing a PGP key that is either invalid or corrupted.  The problem can be fixed by locally signing the imported key:

```
sudo pacman-key --lsign-key AEA0A2E06D592805
```

<br>
