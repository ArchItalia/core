# Core Linux 

![Core Linux Header Image](https://github.com/ArchItalia/site/assets/117321045/3dcdd1a1-e9d2-4dde-bd99-8404541a643b)

## About Core Linux

**Core Linux** is a minimal Linux distribution, based on Arch Linux, that focuses on simplicity and speed. It provides only essential packages for the proper functioning of the OS and is designed for customisation based on the user's needs. Core Linux is only available on 64-bit architectures and is also an official Linux distribution of the Architalia community. 

## Getting Started 

![Screenshot from 2023-08-01 16-11-31](https://github.com/ArchItalia/site/assets/117321045/b2365773-1bd9-4a78-be0b-0d02afb9f46a)

Core Linux is an operating system that requires the entire disk to be used during installation and does not support dual boot. However, it is possible to install it as the first operating system and then resize the available space to create a second partition for another operating system. During installation, Core Linux will prompt you to select the disk to install it on and choose a size for the system, while the rest of the available disk space will be dedicated to the home partition. For example, if the UEFI system is detected, Core Linux will create a 1GB EFI partition, the root partition size will be allocated a certain amount of space, and the remainder will be dedicated to the home partition. Core Linux uses the Btrfs filesystem with subvolumes and a dual partition for both the legacy and UEFI operating systems.

To install Core Linux with its minimal and organised environment, navigate to the **installcore** application in the menu or type `installcore` in the console to start the installation process. You can also import your own guides or scripts to be run through the live based on Arch Linux.

## Configuration
![Screenshot from 2023-08-01 17-09-11](https://github.com/ArchItalia/site/assets/117321045/555c977d-66f3-4f7d-8ebc-5e9bf3a86483)

The customised configuration of Core Linux comes with pre-installed packages such as **yay**, **timeshift**, and **AI-repo**, a repository that has other useful packages. The graphical environment comes with a minimalised version of **Gnome**, that has basic extensions that allow for convenient use. System updates can be managed easily with **Arch Linux updates indicator**, which is configured to handle official packages and AUR through the Core Linux **updates** script. **AppIndicator** allows for the system tray function to appear on the top bar, whereas **Night Theme Switcher** enables automatic switching between light and dark modes. **Desktop-icons-ng** is also available for desktop icons management. Other functions and packages are regularly added to the evolving distribution. 

The filesystem used is **btrfs**, with the creation of subvolumes **@** and **@home**, and **zram generator** is installed for swap management.

![Screenshot from 2023-07-27 20-54-10](https://github.com/ArchItalia/core/assets/117321045/5aebefe1-d4bf-4629-827a-f896bc26df1f)


To ensure the upkeep of the system, use the **clean** tool that is installed and available by typing `clean` in the console.

## Download
[Download](https://drive.google.com/file/d/1dtm1nkgsmDN8l0sxEEgJuCOZn4Xe_BeQ/view?usp=sharing) **Core-ISO-sha256sum.zip** by Architalia GDrive 

!!! warning
   
    requires the entire disk to be used during installation.

!!! info

    - Core Linux
    - version 2023.8 Beta
    - size 1.48G
    - sha256sum fa499652a1f26822fc6147f80b86861637f2028bab3eade8e1a1cf8d0d271f8b



<br>
