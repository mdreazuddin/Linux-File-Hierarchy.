# Linux File Hierarchy Structure.
**The Linux File Hierarchy Structure or the Filesystem Hierarchy Standard (FHS) defines the directory structure and directory contents in Unix-like operating systems. It is maintained by the Linux Foundation.**

<img width="547" alt="image" src="https://github.com/user-attachments/assets/5aedc355-e1dc-41e6-bbd7-12b91ae82dc1">

![Linux File Hierarchy]

_ _ _
## Here, several important Linux files are discussed.

**1. /** - top-level directory.

In Linux, the / (root directory) is the top-level directory where everything on the system is stored. All other files and directories, like /bin, /etc, and /home, are found inside the root directory. Unlike other systems, Linux keeps everything in one place, so all drives and storage are part of this single structure. The / directory is very important because it holds everything needed for the system to work properly.

**2. /root** - is home directory of root.

The /root directory is the home directory for the root user in Linux, who has the highest level of permissions on the system. It is different from the regular user home directories, which are usually located in /home. The /root directory is where the root user’s personal files and settings are stored. It is important to note that this directory should be used carefully, as the root user has full control over the system.
Example:
```
{
cd /root
ls /root
touch /root/newfile.txt
pwd
}
```
These commands demonstrate basic operations in the /root directory, which is typically used for **Supper User** system administration tasks.


**3. /bin** – Essential User Binaries.

The /bin directory contains the fundamental user command binaries that are necessary for the system to operate and be used under single-user mode. Commands like ls, cp, and cat reside here, providing the basic functionality to interact with the filesystem.

**4. /boot** – Boot Loader Files.

/boot stores static bootloader and kernel files needed to boot the operating system. This includes the Linux kernel, initial RAM disk images, and bootloader configuration files like GRUB.

**5. /dev** – Device Files.

This directory contains device files that represent hardware devices and some software interfaces. For instance, /dev/sda represents the first SATA hard drive, and /dev/zero offers a stream of null bytes.

**6. /etc** – Configuration Files.

/etc houses configuration files required by all programs. This includes system-wide configuration files and scripts to start or stop services. The contents of /etc are specific to the local system and change to adjust the system’s behavior.

**7. /home** – User Home Directories.

Each user on the system is assigned a directory in /home, providing a personal space for files, documents, and personal settings. This separation ensures user data is organized and secure.

**8. /lib** – Essential Shared Libraries.

Libraries needed by the binaries in /bin and /sbin are stored in /lib. These shared libraries are crucial for the basic operations of the filesystem, providing common code that can be used by multiple programs.

**9. /media and /mnt** – Mount Points

/media and /mnt are designated for mounting external and temporary filesystems, respectively. /media is typically used for removable media like USB drives, while /mnt can be used for mounting temporary file systems, such as network filesystems or ISO images.

**10. /opt** – Optional Software

The /opt directory is intended for the installation of additional (optional) software that is not part of the default installation. This provides a clear location for third-party applications.

**11. /sbin** – System Administration Binaries

Similar to /bin, /sbin contains essential binaries, but these are intended for system administration rather than general user tasks. Commands like iptables, ifconfig, and fdisk are located here.

**12. /usr** – User Utilities and Applications

One of the largest directories, /usr, is where user utilities and applications are stored. It includes system binaries,documentation, and other non-essential data for running applications.

**13. /var** – Variable Data Files

/var is reserved for files whose content is expected to grow, including logs (/var/log), spooled documents (/var/spool), and temporary files (/var/tmp).


**[Source of conatnt from: Techadmin and others]**
