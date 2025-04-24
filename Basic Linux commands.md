# Command Reference Guide

## File and Directory Operations Commands

| Command | Description                     | Options       | Examples                  |
|---------|---------------------------------|---------------|---------------------------|
| `ls`    | List files and directories.     | `-l`, `-a`, `-h` | `ls -l`                   |
| `mkdir` | Create a new directory.         | `-p`          | `mkdir -p dir1/dir2`      |
| `rm`    | Delete files and directories.   | `-r`, `-f`    | `rm -r dir1`              |
| `cp`    | Copy files and directories.     | `-r`          | `cp -r dir1 dir2`         |
| `mv`    | Move or rename files and directories. |           | `mv file1 file2`          |

## File Permission Commands

| Command | Description                     | Options       | Examples                  |
|---------|---------------------------------|---------------|---------------------------|
| `chmod` | Change file permissions.        | `u`, `g`, `o`, `+`, `-`, `=` | `chmod u+rwx file.txt` |
| `chown` | Change file ownership.          |               | `chown user file.txt`     |
| `chgrp` | Change group ownership.         |               | `chgrp group file.txt`    |
| `umask` | Set default file permissions.   |               | `umask 022`               |

## Process Management Commands

| Command | Description                     | Options       | Examples                  |
|---------|---------------------------------|---------------|---------------------------|
| `ps`    | Display running processes.      | `-aux`        | `ps aux`                  |
| `top`   | Monitor system processes in real-time. |         | `top`                     |
| `kill`  | Terminate a process.            | `-9`          | `kill -9 PID`             |
| `pkill` | Terminate processes based on their name. |       | `pkill process_name`      |
| `pgrep` | List processes based on their name. |           | `pgrep process_name`      |

## System Information Commands

| Command   | Description                     | Options       | Examples                  |
|-----------|---------------------------------|---------------|---------------------------|
| `uname`   | Display system information.     | `-a`          | `uname -a`                |
| `hostname`| Display the system's hostname.  |               | `hostname`                |
| `uptime`  | Display system uptime.          |               | `uptime`                  |
| `lscpu`   | Display CPU information.        |               | `lscpu`                   |
| `lsusb`   | List USB devices.               |               | `lsusb`                   |

## Networking Commands

| Command   | Description                     | Options       | Examples                  |
|-----------|---------------------------------|---------------|---------------------------|
| `ifconfig`| Display network interface information. |         | `ifconfig`                |
| `ping`    | Send ICMP echo requests to a host. |           | `ping google.com`         |
| `netstat` | Display network connections and statistics. | `-tuln` | `netstat -tuln`           |
| `ss`      | Display network socket information. | `-tuln`   | `ss -tuln`                |
| `ssh`     | Securely connect to a remote server. |         | `ssh user@hostname`       |
| `scp`     | Securely copy files between hosts. |           | `scp file.txt user@hostname:/path/to/destination` |
| `wget`    | Download files from the web.    |               | `wget http://example.com/file.txt` |
| `curl`    | Transfer data to or from a server. |           | `curl http://example.com` |

```
