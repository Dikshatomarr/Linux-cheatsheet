# Linux-cheatsheet

Some useful Linux commands organized by categories in a cheat sheet format:

### Basic Commands:
- `pwd` - Print working directory (current location)
- `ls` - List directory contents
  - `ls -l` - Long listing format
  - `ls -a` - Show hidden files
- `cd [directory]` - Change directory
- `mkdir [dir_name]` - Create a new directory
- `rm [file_name]` - Remove a file
  - `rm -r [dir_name]` - Remove a directory and its contents
- `cp [source] [destination]` - Copy files/directories
  - `cp -r [source] [destination]` - Recursively copy directories
- `mv [source] [destination]` - Move or rename files/directories
- `touch [file_name]` - Create a new file
- `cat [file_name]` - Display file contents
- `more [file_name]` - View file content page by page
- `head [file_name]` - Show first 10 lines of a file
- `tail [file_name]` - Show last 10 lines of a file
  - `tail -f [file_name]` - Continuously output appended data (useful for logs)

### File Permissions:
- `chmod [permissions] [file_name]` - Change file permissions
  - `chmod 755 [file_name]` - Assign read/write/execute permissions to user, and read/execute to group/others
- `chown [user]:[group] [file_name]` - Change file owner and group

### File Compression:
- `tar -cvf [archive.tar] [file]` - Create a tarball
- `tar -xvf [archive.tar]` - Extract a tarball
- `gzip [file_name]` - Compress a file
- `gunzip [file_name.gz]` - Decompress a file

### Process Management:
- `ps` - Show running processes
- `top` - Display live system processes and resource usage
- `kill [PID]` - Terminate a process by its ID
  - `kill -9 [PID]` - Force terminate a process
- `bg` - Run a process in the background
- `fg` - Bring a process to the foreground

### Networking:
- `ifconfig` - Show network interfaces and IP addresses
- `ping [host]` - Check network connectivity to a host
- `netstat` - Network statistics (like open connections)
- `curl [URL]` - Send request to a URL
- `wget [URL]` - Download files from the web

### Disk Usage:
- `df -h` - Display disk space usage
- `du -sh [directory]` - Show the size of a directory

### User Management:
- `whoami` - Show current username
- `sudo [command]` - Run command with superuser privileges
- `adduser [username]` - Add a new user
- `passwd [username]` - Change user password
- `who` - Show who is logged in

### System Information:
- `uname -a` - Show system information (kernel version, architecture)
- `uptime` - Show how long the system has been running
- `dmesg` - Kernel message buffer (useful for troubleshooting)
- `free -h` - Show memory usage
- `lscpu` - Show CPU architecture info
- `lsblk` - List block devices (disks and partitions)

### Package Management (Ubuntu/Debian-based systems):
- `apt update` - Update the package list
- `apt upgrade` - Install available upgrades
- `apt install [package_name]` - Install a package
- `apt remove [package_name]` - Remove a package

### Text Editors:
- `nano [file_name]` - Open file in Nano editor
- `vim [file_name]` - Open file in Vim editor

### Log Files:
- `/var/log/syslog` - System log
- `/var/log/auth.log` - Authentication log
- `/var/log/dmesg` - Kernel ring buffer log
