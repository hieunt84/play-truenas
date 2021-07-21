### Intro
    deploy TrueNAS CORE

### Prepare
    VM: BSD > FreeBSD 64bit
      vCPUs: 2
      RAM: 8GB
      Controller IDE: CDROM
      Controller: ISCI
        HDD1: 16GB for os truenas
        HDD2: NVMe 18GB for cache
        HDD2: 16GB
        HDD3: 16GB
        HDD4: 16GB
      Nic1: Bridged
      IP: 172.20.10.110
      root/abc123xxx

### Deploy
    1.Download true nas
      https://www.truenas.com/download-truenas-core/

    2.Install
    
    3.Config Static IP
      Goto : Network > Interface > em0 > edit
        - uncheck DHCP
        - set ip static
        - test changes
   <p align="center"><img src="https://github.com/hieunt84/play-truenas/blob/master/images/config-network.PNG" /></p>

    4.Config DNS & Defaut Gateway
      Goto : Network > Global Configuration
        - set dns
        - set default gateway
   <p align="center"><img src="https://github.com/hieunt84/play-truenas/blob/master/images/config-network-3.PNG" /></p>
    
### Ref
    https://www.truenas.com/docs/core/gettingstarted/install/
    https://www.ods.vn/tai-lieu/gioi-thieu-va-huong-dan-cai-dat-he-dieu-hanh-freenas.html
    https://www.youtube.com/watch?v=nVRWpV2xyds&list=WL&index=4&t=419s
    https://www.youtube.com/watch?v=17ZWLxrGrCA
