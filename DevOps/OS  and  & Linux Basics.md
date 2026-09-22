# DevOps Fundamentals — OS & Linux Basics

## 1. Operating System (OS)

### What is an Operating System?

An **Operating System (OS)** is system software that manages the computer's hardware and provides a platform for applications to run.

Examples:

- Windows
- Linux
- macOS
- Android
- iOS

### What does an OS manage?

An OS manages:

- CPU
- Memory (RAM)
- Storage
- Files and directories
- Processes
- Users
- Network
- Hardware/devices
- Security and permissions

### Simple Example

```text
Java Application
       ↓
Operating System
       ↓
CPU + RAM + Storage

# DevOps — Server to Linux Processes

---
```

# 1. Server

## What is a Server?

A **server is a computer that provides services or resources to other computers or applications over a network.**

A server is not necessarily a special type of computer. A normal computer can act as a server if it provides a service.

### Examples of What a Server Can Run

- Web applications
- Java applications
- APIs
- Databases
- File storage
- Authentication systems

### Simple Example

```text
Your Browser
     ↓
Internet / Network
     ↓
Web Server
     ↓
Application
     ↓
Database

```
# DevOps — Server to Linux Processes

---

## 2. Server

A **server** is a computer or system that provides services, applications, or resources to other computers called **clients**.

In DevOps, servers are commonly used to:
- Run applications
- Store data
- Host websites
- Run databases
- Handle network requests

---

## 3. Linux

**Linux** is an open-source operating system kernel.

In everyday usage, the term "Linux" is also commonly used to refer to operating systems built around the Linux kernel.

Linux is widely used on:
- Servers
- Cloud infrastructure
- Containers
- Virtual machines
- Development environments

---

## 4. Linux Kernel

The **Linux Kernel** is the core part of the Linux operating system.

It manages communication between:
- Hardware
- Applications
- System resources

The kernel manages resources such as:
- CPU
- Memory
- Processes
- Devices
- Filesystems

---

## 5. Linux Distribution

A **Linux distribution (distro)** is a complete operating system built around the Linux kernel.

A distribution usually contains:
- Linux kernel
- System utilities
- Package manager
- Shell
- Applications
- Configuration tools

Examples:
- Ubuntu
- Debian
- Fedora
- Red Hat Enterprise Linux (RHEL)
- Rocky Linux
- Amazon Linux

---

## 6. GUI

**GUI (Graphical User Interface)** allows users to interact with a computer using graphical elements such as:
- Windows
- Icons
- Buttons
- Menus
- Mouse

---

## 7. CLI

**CLI (Command Line Interface)** allows users to interact with a computer by entering text commands.

DevOps engineers commonly use the CLI to:
- Manage servers
- Install software
- Manage files
- Monitor systems
- Run applications
- Automate tasks

---

## 8. Terminal

A **terminal** is a program/interface through which you can interact with a computer using the command line.

The terminal provides a place where you can enter commands and see their output.

---

## 9. Shell

A **shell** is a command interpreter.

It receives commands from the user, interprets them, and communicates with the operating system to perform the requested task.

---

## 10. Bash

**Bash (Bourne Again SHell)** is one of the most commonly used shells on Linux systems.

It allows users to:
- Execute commands
- Work with files
- Manage processes
- Run scripts
- Automate tasks

---

# Linux File System

## 11. Linux File System

The **Linux filesystem** is the hierarchical structure used to organize files and directories in Linux.

Unlike Windows, Linux uses a single directory tree that starts from the **root directory `/`**.

---

## 12. Root Directory `/`

The **root directory `/`** is the starting point of the Linux filesystem.

All other directories and files exist somewhere under `/`.

---

## 13. `/home`

`/home` contains the personal directories of normal users.

Each user generally has their own home directory for storing personal files and configurations.

---

## 14. `/etc`

`/etc` contains system-wide configuration files.

It is mainly used for configuring:
- Services
- Applications
- System settings

---

## 15. `/var`

`/var` contains data that changes frequently while the system is running.

It commonly contains:
- Logs
- Application data
- Cache
- Spool files

---

## 16. `/tmp`

`/tmp` is used for temporary files created by applications and users.

Temporary data is generally stored here for short-term use.

---

## 17. `/usr`

`/usr` contains many user-level programs, libraries, documentation, and other system resources.

---

## 18. `/dev`

`/dev` contains special files that represent devices connected to or managed by the system.

Examples include representations of:
- Disks
- Terminals
- Other hardware devices

---

## 19. `/proc`

`/proc` is a virtual filesystem that provides information about the running system and processes.

It contains information related to:
- Processes
- CPU
- Memory
- Kernel

---

# Files and Directories

## 20. File

A **file** is a container used to store data.

Examples of data stored in files include:
- Text
- Configuration
- Logs
- Source code
- Application data

---

## 21. Directory

A **directory** is a container used to organize files and other directories.

It is similar to a folder in Windows.

---

# Linux Users

## 22. User

A **user** is an account that can interact with and access resources on a Linux system.

Different users can have different permissions.

---

## 23. Root User

The **root user** is the administrator account in Linux.

Root has very high-level privileges and can perform almost any operation on the system.

---

## 24. `sudo`

**sudo** stands for **SuperUser Do**.

It allows an authorized normal user to execute a command with elevated privileges.

---

## 25. Group

A **group** is a collection of users.

Groups are used to manage permissions for multiple users efficiently.

---

# Linux Permissions

## 26. Permissions

**Linux permissions** control who can access or modify files and directories.

Permissions are mainly assigned to:

- Owner
- Group
- Others

---

## 27. Read Permission

**Read (`r`)** permission allows a user to view the contents of a file.

For a directory, read permission allows the user to see the directory's contents.

---

## 28. Write Permission

**Write (`w`)** permission allows a user to modify a file.

For a directory, write permission allows changes to its contents.

---

## 29. Execute Permission

**Execute (`x`)** permission allows a file to be executed.

For a directory, execute permission allows a user to access/traverse the directory.

---

## 30. `chmod`

**chmod** is used to change the permissions of files and directories.

The name comes from **change mode**.

---

## 31. `chown`

**chown** is used to change the ownership of a file or directory.

The name comes from **change owner**.

---

# Linux Processes

## 32. Process

A **process** is a running instance of a program.

When a program starts executing, the operating system creates a process for it.

A process uses system resources such as:
- CPU
- Memory
- Files
- Network resources

---

## 33. PID

**PID (Process ID)** is a unique number assigned to a running process by the operating system.

The PID is used to identify and manage a specific process.

---

## 34. Foreground Process

A **foreground process** is a process that runs directly in the current terminal session and interacts with the user.

The terminal normally waits for the foreground process to finish.

---

## 35. Background Process

A **background process** runs without requiring the terminal to actively wait for it.

This allows the user to continue using the terminal while the process keeps running.

---

## 36. Program vs Process

### Program

A **program** is a set of instructions stored on disk.

### Process

A **process** is a program that is currently running.

**Simple idea:**

Program = stored instructions

Process = running instructions

---

## 37. Why Processes Matter in DevOps

Processes are important in DevOps because applications and services run as processes on servers.

A DevOps engineer needs to understand processes to:
- Monitor applications
- Identify running services
- Check resource usage
- Troubleshoot problems
- Stop or restart applications
- Maintain server availability

---

# Map

Server
↓
Linux
↓
Linux Kernel
↓
Linux Distribution
↓
Terminal
↓
Shell
↓
Commands
↓
Linux Filesystem
↓
Users
↓
Permissions
↓
Processes
↓
DevOps Server Management
