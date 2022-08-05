# 1. common system administrator command

1. hard disk
    - lsblk: list devices, like partitions;
    - df: device usage; `df -h` （human-readable）;
    - mount:  mount partition, `mount /dev/sdb1 /mnt/usb`;
1. process
    - ps: running process information;
        - e: every process;
        - f: full information;
        - `ps -ef | grep firefox`
    - kill: kill a process, `kill pid`;
    - top/htop: more readable display system information;
1. memory: free
    1. free -m: megabytes;
    1. free: unused memory;
    1. available: free + part of buff/cache;
1. network
    - ip: show ip related information;
        - ip addr (ip a);
    - ping: test networking;
    - ss: show socket information
        - `ss -ant`: show all tcp connection on you computer;
