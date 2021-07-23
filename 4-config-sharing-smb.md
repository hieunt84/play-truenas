### Config share SMB    
    1.Create user/group
      Goto: Account > User > ADD
        - create group first.
        - create user after.

    2.Create dataset (folder chứa data company) from Pool Storage
      Goto: Storage> Pool > : > Add Dataset
         - Share type: SMB  

    3.Config permision
      Goto: Storage> Pool > Dataset > : Edit Permissions
        - giữ quyền default của hệ thống.    

    4.Config Sharing SMB
      Goto: Sharing > Window Shares(SMB) > ADD
        - set sharename: my company
  <p align="center"><img src="https://github.com/hieunt84/play-truenas/blob/master/images/sharing-smb.PNG" /></p>

    5.Enable Shadow Copy
      Default enable in setp config sharing smb above.  
        
    6.Config quotas if need
      Goto: Pool > Storage > Pool > Dataset > : > User Quotas
    
    7.Testing

    8.Config permission on demand
      -Goto: Storage> Pool > Dataset > : Edit Permissions
        - set account admin full control dataset.     
        - remove group @everyone.
        - edit permission group builtin-user : Read.

      -Map disk share with account full control.
      -Using gui on window to config permission on demand.
  <p align="center"><img src="https://github.com/hieunt84/play-truenas/blob/master/images/config-permission.PNG" /></p>

### Ref
    ref: https://www.ixsystems.com/blog/windows-smb-shares-on-freenas/