# Linux API Documentation
[![Reddit](https://img.shields.io/badge/Reddit-FF4500?style=for-the-badge&logo=reddit&logoColor=white)](https://www.reddit.com/r/linux_programming/new/)
[![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)](https://elixir.bootlin.com/linux/v6.17/source)
<p align="center">
    <a href="https://github.com/cybersecurity-dev/"><img height="25" src="https://github.com/cybersecurity-dev/cybersecurity-dev/blob/main/assets/github.svg" alt="GitHub"></a>
    &nbsp;
    <a href="https://www.youtube.com/@CyberThreatDefence"><img height="25" src="https://github.com/cybersecurity-dev/cybersecurity-dev/blob/main/assets/youtube.svg" alt="YouTube"></a>
    &nbsp;
    <a href="https://cyberthreatdefence.com/my_awesome_lists"><img height="20" src="https://github.com/cybersecurity-dev/cybersecurity-dev/blob/main/assets/blog.svg" alt="My Awesome Lists"></a>
    <img src="https://github.com/cybersecurity-dev/cybersecurity-dev/blob/main/assets/bar.gif">
</p>


## 📖 Contents
- [My Awesome Lists](#my-awesome-lists)
- [Contributing](#contributing)
- [Contributors](#contributors)


| Category               | Description                                                                                                                            | Key System Calls                                                                                                                                                                                                                                                                                                                         |
| :--------------------- | :------------------------------------------------------------------------------------------------------------------------------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Process Management** | System calls for creating, controlling, and terminating processes.                                                                     | `fork`, `execve`, `waitpid`, `exit`, `kill`, `getpid`, `getppid`, `nice`, `sched_setscheduler`, `sched_getscheduler`                                                                                                                                                                                                                          |
| **Memory Management** | System calls for allocating and managing memory regions.                                                                                | `mmap`, `munmap`, `brk`, `sbrk`, `mprotect`, `mlock`, `munlock`                                                                                                                                                                                                                                                                       |
| **File System** | System calls for interacting with files and directories.                                                                               | `open`, `close`, `read`, `write`, `lseek`, `stat`, `fstat`, `access`, `chmod`, `chown`, `truncate`, `unlink`, `mkdir`, `rmdir`, `rename`, `link`, `symlink`, `readlink`, `mount`, `umount`                                                                                                                                                |
| **Inter-Process Communication (IPC)** | System calls that allow different processes to communicate and synchronize with each other.                                 | **Pipes:** `pipe`, **Message Queues:** `msgget`, `msgsnd`, `msgrcv`, `msgctl`, **Shared Memory:** `shmget`, `shmat`, `shmdt`, `shmctl`, **Semaphores:** `semget`, `semop`, `semctl`, **Sockets:** `socket`, `bind`, `listen`, `accept`, `connect`, `send`, `recv`, `close` (also used for network communication) |
| **Signal Handling** | System calls for managing signals, which are asynchronous notifications sent to a process to indicate events.                              | `signal`, `sigaction`, `kill`, `raise`, `pause`, `sigprocmask`, `sigsuspend`, `sigpending`                                                                                                                                                                                                                                            |
| **Device I/O** | System calls for interacting with hardware devices. Files are often used as an abstraction for devices in Linux.                          | `ioctl` (general device control), `read`, `write` (on device files), `mmap` (for memory-mapped device I/O)                                                                                                                                                                                                                             |
| **Networking** | System calls specifically for network communication. (Note: Sockets are also a form of IPC).                                            | `socket`, `bind`, `listen`, `accept`, `connect`, `send`, `recv`, `sendto`, `recvfrom`, `getsockname`, `getpeername`, `setsockopt`, `getsockopt`, `shutdown`                                                                                                                                                                               |
| **Time Management** | System calls for getting and setting the system time and timers.                                                                         | `time`, `gettimeofday`, `settimeofday`, `nanosleep`, `alarm`, `timer_create`, `timer_settime`, `timer_gettime`, `timer_delete`                                                                                                                                                                                                           |
| **User and Group IDs** | System calls for getting and setting user and group identifiers associated with a process.                                                 | `getuid`, `geteuid`, `setuid`, `seteuid`, `getgid`, `getegid`, `setgid`, `setegid`, `getgroups`, `setgroups`                                                                                                                                                                                                                          |
| **System Information** | System calls for retrieving various information about the system.                                                                       | `uname`, `gethostname`, `sysinfo`, `sysconf`, `pathconf`                                                                                                                                                                                                                                                                             |
| **Security** | System calls related to security features and access control.                                                                           | `chmod`, `chown`, `access`, `setuid`, `seteuid`, `setgid`, `setegid`, `capget`, `capset` (capabilities), `prctl` (process control with security-related options)                                                                                                                                                                              |
| **Real-time Extensions** | System calls that provide real-time scheduling and memory locking capabilities.                                                           | `sched_setscheduler` (with real-time policies), `sched_getparam`, `sched_setparam`, `mlock`, `munlock`, `mlockall`, `munlockall`, `timer_create` (with `CLOCK_REALTIME` or `CLOCK_MONOTONIC`), `timer_settime`                                                                                                                             |



## 

### My Awesome Lists
You can access the my awesome lists [here](https://cyberthreatdefence.com/my_awesome_lists)

### Contributing
[Contributions of any kind welcome, just follow the guidelines](contributing.md)!

### Contributors
[Thanks goes to these contributors](https://github.com/cybersecurity-dev/awesome-linux-internals/graphs/contributors)!

[🔼 Back to top](#awesome-linux-internals-)
