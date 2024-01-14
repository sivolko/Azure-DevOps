---
description: aka Linux Terminal,  CL
---

# ⚠ Shell

* Shell provides a text-based input/output (I/O) interface between <mark style="color:red;">**users**</mark> and the <mark style="color:red;">**Kernel**</mark> for a computer system.
* Console is not a window, but it's a screen in text mode.
* Terminal is a window but console is not&#x20;

### <mark style="color:purple;">Terminal Emulators</mark>

Terminal Emulator is a s/w that emulates the function of a terminal.

* It allows the use of text-based programs within a GUI (Graphical User Interface)
* It's also called as CLI because CLI that run as additional terminals in one terminal.
* Terminal serves as an interface to the shell interpreter.

<figure><img src="../../.gitbook/assets/image (1).png" alt=""><figcaption><p>Terminal Emulator </p></figcaption></figure>

### <mark style="color:purple;">**Types of Shell**</mark>

1. BASH (Bourne-Again Shell)
2. SSH&#x20;
3. Tcsh/Csh
4. Ksh
5. Zsh
6. Fish

### <mark style="color:purple;">Unprivileged - User Shell Prompt</mark>

<figure><img src="../../.gitbook/assets/image (2).png" alt=""><figcaption><p>$ indicates normal user </p></figcaption></figure>

### <mark style="color:purple;">**Privileged - Root Shell Prompt**</mark>

<figure><img src="../../.gitbook/assets/image (3).png" alt=""><figcaption><p>#indicates logged as privileged user</p></figcaption></figure>

### <mark style="color:purple;">System Information</mark>

| **Command** | **Description**                                                                                                                    |
| ----------- | ---------------------------------------------------------------------------------------------------------------------------------- |
| `whoami`    | Displays current username.                                                                                                         |
| `id`        | Returns users identity                                                                                                             |
| `hostname`  | Sets or prints the name of current host system.                                                                                    |
| `uname`     | Prints basic information about the operating system name and system hardware.                                                      |
| `pwd`       | Returns working directory name.                                                                                                    |
| `ifconfig`  | The ifconfig utility is used to assign or to view an address to a network interface and/or configure network interface parameters. |
| `ip`        | Ip is a utility to show or manipulate routing, network devices, interfaces and tunnels.                                            |
| `netstat`   | Shows network status.                                                                                                              |
| `ss`        | Another utility to investigate sockets.                                                                                            |
| `ps`        | Shows process status.                                                                                                              |
| `who`       | Displays who is logged in.                                                                                                         |
| `env`       | Prints environment or sets and executes command.                                                                                   |
| `lsblk`     | Lists block devices.                                                                                                               |
| `lsusb`     | Lists USB devices                                                                                                                  |
| `lsof`      | Lists opened files.                                                                                                                |
| `lspci`     | Lists PCI devices.                                                                                                                 |

### <mark style="color:purple;">Logging In via SSH</mark>

```bash
ssh [username]@[IP address]
```

