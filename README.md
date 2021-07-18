# play-truenas
### Intro
    - for backup
    - creat digital workspace, access from inside and outside company.
### Prepare
    VM:
      vCPUs: 2
      RAM: 8GB
      HDD1: 8GB for os true nas
      HDD2: 20GB for storage
      Nic1: 1GB
      IP: 172.20.10.110
      root/abcxxx
### Deploy
    1.Download true nas
      https://www.truenas.com/download-truenas-core/      
    2.Install
    3.Config Static IP
      Go to : Network > Interface > em0
   <p align="center"><img src="https://github.com/hieunt84/play-truenas/blob/master/images/config-network2.PNG" /></p>
      Go to : Network > Global Configuration > se DNS & Defaut Gateway
      
    4.Make pool
      Go to: Storage > Pool > Add
   <p align="center"><img src="https://github.com/hieunt84/play-truenas/blob/master/images/add-pool.PNG" /></p>

### Ref
    https://www.ods.vn/tai-lieu/gioi-thieu-va-huong-dan-cai-dat-he-dieu-hanh-freenas.html
