# Core Linux 

Core Linux is a new distribution based on Arch Linux, developed by the Italian community Architalia. It is described as a friendly, powerful, and easy-to-use distribution. Its installation is done through a configuration script that guides the user in choosing the system configuration options.


The script starts by asking for the language to use during installation and shows a brief description of the project and the community that develops it. Then, it enters a series of guided choices to configure the system, starting with the selection of language, time zone, and character map.

The process continues with the choice of the username, which is used to create the user account, the user password, and the root password encrypted with a securely generated key. The user can also choose one of the three available shells: bash, zsh, or fish.

Next, the user is guided to choose among four possible AUR helpers and four possible firewalls: firewalld, ufw, iptables, or none. In addition, it's possible to choose the standard linux kernel or other versions such as linux-lts, linux-zen, linux-hardened, each with different features.

Once some choices are made about which packages to install and which base version to select, the configuration of the disk partition is reached, where it is possible to choose the device on which to install the operating system, the file system format, and the partition size.

The installation continues with the choice of the swap partition size. Then it's asked to select the nearest server mirror, and finally, an overview of all the choices made is presented. Here the user can choose to confirm and proceed with the installation or go back to the configuration phase to make changes.

Finally, the script starts the actual installation, using the configuration file created earlier. The system installation will take some time depending on the power of the user's computer and the number of selected packages.

In summary, Core Linux is an Arch Linux-based distribution designed to be friendly, powerful, and easy to use. The installation script provides a guided and simplified experience, allowing the user to customize their system securely and quickly.

Clean is a tool created by the Core Linux team developers for system maintenance to remove orphan packages, package cache, user cache, and trash. Just type the clean command or use the application in the menu.

The main difference between the Minimal and Full versions of Core Linux is related to the packages included in the basic installation. The Minimal version includes only the essential packages necessary to make the operating system work, such as the Arch Linux base core, libraries, fonts, themes, the Xorg graphical client, the GNOME desktop environment with some accessories like Nautilus, the network manager, the CUPS printing utility, and other utility packages like cronie and Git.

In the Full version, instead, we also find packages like LibreOffice (an open-source alternative to Microsoft Office), Blender and Inkscape (3D graphics and animation programs), GIMP (a powerful image editor), VLC (a media player), and many other useful tools such as advanced text editors, productivity programs, applications for contact management, system utilities, communication applications, and many others.

For both versions, the user can choose the type of AUR helper, firewall, and shell to use. Also, the installation requires the user to select a mirror server and the kernel version to use.

In general, the Minimal version is designed to provide a solid foundation for building a customized operating system, while the Full version is more complete and offers many ready-to-use features for the average user. However, with both versions, the user has the flexibility to further customize their system according to their needs and preferences.

Base packages in the Minimal Version:

```
* core-base
* architalia-fonts
* core-gtk-theme
* core-gnome-backgrounds
* core-icons-theme
* core-keyring
* core-extensions-base
* core-terminal-nord-theme
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


## Download
[Download](#) coming soon..

!!! warning
   
    requires the entire disk to be used during installation.

!!! info

    - Core Linux
    - installcore v1.9
    - version 2023.8 Beta
    - size 1.48G
    - sha256sum 

NOTE: Pacman will complain about importing a PGP key that is either invalid or corrupted.  The problem can be fixed by locally signing the imported key:

```
sudo pacman-key --lsign-key AEA0A2E06D592805
```

<br>
