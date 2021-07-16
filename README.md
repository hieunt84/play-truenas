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
   <p align="center"><img src="https://github.com/hieunt84/play-truenas/blob/master/images/Config-network.PNG" /></p>

    4.Make pool
      Go to: Storage > Pool > Add
   <p align="center"><img src="https://github.com/hieunt84/play-truenas/blob/master/images/add-pool.PNG" /></p>

### Config share SMB
    ref: https://www.ixsystems.com/blog/windows-smb-shares-on-freenas/
   <p align="center"><img src="https://github.com/hieunt84/play-truenas/blob/master/images/sharing-smb.PNG" /></p>

    - Create user/group
    - shadow copy (default)
    - permision
      Go to: Pool > Storage > Pool1 > Windowset > : > Edit Permisions
    - quotas
      Go to: Pool > Storage > Pool1 > Windowset > : > User Quotas
   
