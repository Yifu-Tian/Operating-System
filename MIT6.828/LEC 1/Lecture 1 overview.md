# Overview
## 这门课的两个目标:
1. 理解操作系统的设计与实现
2. 上手做一个小的O/S(谁不想自己做一个操作系统呢~)

## os设计方法
往小看: 一个硬件管理库\
往大看: 物理机器->抽象一个更好的属性

# 组织
h/w: CPU, mem, disk, &c
kernel services
user applications: vi, gcc, &c

# What services does an O/S kernel typically provide?
* processes
* memory allocation
* file contents
* directories and file names
* security
* many others: users, IPC, network, time, terminals

# 一个操作系统抽象看起来是什么样子的?
* Applications see them only via system calls
* Examples, from UNIX (e.g. Linux, OSX, FreeBSD):

            fd = open("out", 1);
            write(fd, "hello\n", 6);
            pid = fork();
