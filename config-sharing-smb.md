### Config share SMB    
   <p align="center"><img src="https://github.com/hieunt84/play-truenas/blob/master/images/sharing-smb.png" /></p>

    - Create user/group
      Goto: Account > User > ADD
    - Create dataset from Pool Storage
      Goto: Storage> Pool > : > Add Dataset
    - Config permision
      Goto: Storage> Pool > Dataset > : Edit Permissions
    - Config Sharing SMB
      Goto: Sharing > Window Shares > ADD
        shadow copy (default)    
    - Config quotas
      Goto: Pool > Storage > Pool > Dataset > : > User Quotas


### Ref
    ref: https://www.ixsystems.com/blog/windows-smb-shares-on-freenas/