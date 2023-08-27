# In this repo you can find attempt to use SO_ATTACH_REUSEPORT_CBPF to load balance traffic between threads.

This code is not working. It was published just to highlight issue in Linux kernel.

This is example code for my blog [article](https://pavel.network/rocky-road-towards-ultimate-udp-load-balancing-server-on-linux/)

Example output:
```
We will listen on :::2055 udp port
Setting reuse port
Loading BPF to implement random UDP traffic distribution over available threads
Successfully loaded reuse port BPF
Successful bind
We will listen on :::2055 udp port
Setting reuse port
Loading BPF to implement random UDP traffic distribution over available threads
Successfully loaded reuse port BPF
Can't bind on port: 2055 on host :: errno:98 error: Address already in use
Cannot create / bind socket
Started capture
```

Platform:
```
Ubuntu 22.04, 6.2.0-26-generic
```
