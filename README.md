# Homework 10.3

Задание 1

![1](https://raw.githubusercontent.com/Evgeniy-Nikolskiy/hw10.3/main/assets/1031.png)

Задание 2 и 3

LA 1/5/15  
```
node_load1{job="nodeexporter"}  
node_load5{job="nodeexporter"}  
node_load15{job="nodeexporter"}  
```
CPU Usage (%)  
```
100 - (avg by (instance) (rate(node_cpu_seconds_total{job="nodeexporter",mode="idle"}[1m])) * 100)  
```
Memory Availible (%)  
```
node_memory_Inactive_bytes / node_memory_MemAvailable_bytes*100  
```
Free Space on FS (%)  
```
node_filesystem_avail_bytes{fstype!~"tmpfs|fuse.lxcfs|squashfs"} / node_filesystem_size_bytes{fstype!~"tmpfs|fuse.lxcfs|squashfs"}*100  
```
![2](https://raw.githubusercontent.com/Evgeniy-Nikolskiy/hw10.3/main/assets/1032.png)

