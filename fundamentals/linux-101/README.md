---
description: This module is created with reference of HTB Linux Sandbox
layout:
  title:
    visible: true
  description:
    visible: true
  tableOfContents:
    visible: true
  outline:
    visible: false
  pagination:
    visible: true
---

# 🐧 Linux 101

## <mark style="color:purple;">History and Key Points</mark>

* Free Open-Source Kernel&#x20;
* started as personal project in 1991 by Linus Torvalds
* Comes under GNU General Public License v2
* 600 distributions available eg- Ubuntu, Debian, Fedora , Kali, Parrot OS

<img src="../../.gitbook/assets/file.excalidraw.svg" alt="Basic structure of OS " class="gitbook-drawing">

### <mark style="color:purple;">5 Principles of Linux</mark>&#x20;

| Principle                                                       | Description                                                                                                                                                   |
| --------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Everything is a file**                                        | All configuration files for the various services running on the Linux operating system are stored in one or more text files.                                  |
| **Small, Single-purpsose Program**                              | Linux offers many different tools that we will work with, which can be combined to work together.                                                             |
| **Ability to chain programs together to perform complex tasks** | The integration and combination of different tools enable us to carry out many large and complex tasks, such as processing or filtering specific data results |
| **Avoid captive user interfaces**                               | Linux is designed to work mainly with the shell (or terminal), which gives the user greater control over the operating system.                                |
| **Configuration data stored in a text file**                    | An example of such a file is the `/etc/passwd` file, which stores all users registered on the system.                                                         |

### Linux Architecture

The Linux operating system can be broken down into layers:

| Layer              | Description                                                                                                                                                                                                                                                                                        |
| ------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Hardware**       | Peripheral devices such as the system's RAM, hard drive, CPU, and others                                                                                                                                                                                                                           |
| **Kernel**         | The core of the Linux operating system whose function is to virtualize and control common computer hardware resources like CPU, allocated memory, accessed data, and others. The kernel gives each process its own virtual resources and prevents/mitigates conflicts between different processes. |
| **Shell**          | A command-line interface (CLI), aka a shell that a user can enter commands into to execute the kernel's functions.                                                                                                                                                                                 |
| **System utility** | Makes available to the user all of the operating system's functionality.                                                                                                                                                                                                                           |

### <mark style="color:purple;">Components</mark>

| Component           | Description                                                                                                                                                                                                                                                                                                                                     |
| ------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Bootloader**      | A piece of code that runs to guide the booting process to start the operating system. Parrot Linux uses the GRUB Bootloader.                                                                                                                                                                                                                    |
| **OS kernel**       | The kernel is the main component of an operating system. It manages the resources for system's I/O devices at the hardware level.                                                                                                                                                                                                               |
| **Daemons**         | Background services are called "daemons" in Linux. Their purpose is to ensure that key functions such as scheduling, printing, and multimedia are working correctly. These small programs load after we booted or log into the computer                                                                                                         |
| **OS Shell**        | The operating system shell or the command language interpreter (also known as the command line) is the interface between the OS and the user. This interface allows the user to tell the OS what to do. The most commonly used shells are Bash, Tcsh/Csh, Ksh, Zsh, and Fish.                                                                   |
| **Graphics server** | This provides a graphical sub-system (server) called "X" or "X-server" that allows graphical programs to run locally or remotely on the X-windowing system                                                                                                                                                                                      |
| **Window Manager**  | Also known as a graphical user interface (GUI). There are many options, including GNOME, KDE, MATE, Unity, and Cinnamon. A desktop environment usually has several applications, including file and web browsers. These allow the user to access and manage the essential and frequently accessed features and services of an operating system. |
| **Utilities**       | Applications or utilities are programs that perform particular functions for the user or another program.                                                                                                                                                                                                                                       |

### <mark style="color:purple;">File System Hierarchy</mark>

The Linux operating system is structured in a tree-like hierarchy and is documented in the [Filesystem Hierarchy](http://www.pathname.com/fhs/) Standard (FHS). Linux is structured with the following standard top-level directories

Now Linux Foundation takes care of FSH V3.0 released in 2015&#x20;

[https://refspecs.linuxfoundation.org/FHS\_3.0/fhs-3.0.pdf](https://refspecs.linuxfoundation.org/FHS\_3.0/fhs-3.0.pdf)

<figure><img src="../../.gitbook/assets/image.png" alt=""><figcaption><p>Source : HTB</p></figcaption></figure>

<table data-header-hidden><thead><tr><th width="228"></th><th></th></tr></thead><tbody><tr><td><strong>Path</strong></td><td><strong>Description</strong></td></tr><tr><td><code>/</code></td><td>The top-level directory is the root filesystem and contains all of the files required to boot the operating system before other filesystems are mounted as well as the files required to boot the other filesystems. After boot, all of the other filesystems are mounted at standard mount points as subdirectories of the root.</td></tr><tr><td><code>/bin</code></td><td>Contains essential command binaries.</td></tr><tr><td><code>/boot</code></td><td>Consists of the static bootloader, kernel executable, and files required to boot the Linux OS.</td></tr><tr><td><code>/dev</code></td><td>Contains device files to facilitate access to every hardware device attached to the system.</td></tr><tr><td><code>/etc</code></td><td>Local system configuration files. Configuration files for installed applications may be saved here as well.</td></tr><tr><td><code>/home</code></td><td>Each user on the system has a subdirectory here for storage.</td></tr><tr><td><code>/lib</code></td><td>Shared library files that are required for system boot.</td></tr><tr><td><code>/media</code></td><td>External removable media devices such as USB drives are mounted here.</td></tr><tr><td><code>/mnt</code></td><td>Temporary mount point for regular filesystems.</td></tr><tr><td><code>/opt</code></td><td>Optional files such as third-party tools can be saved here.</td></tr><tr><td><code>/root</code></td><td>The home directory for the root user.</td></tr><tr><td><code>/sbin</code></td><td>This directory contains executables used for system administration (binary system files).</td></tr><tr><td><code>/tmp</code></td><td>The operating system and many programs use this directory to store temporary files. This directory is generally cleared upon system boot and may be deleted at other times without any warning.</td></tr><tr><td><code>/usr</code></td><td>Contains executables, libraries, man files, etc.</td></tr><tr><td><code>/var</code></td><td>This directory contains variable data files such as log files, email in-boxes, web application related files, cron files, and more.</td></tr></tbody></table>

