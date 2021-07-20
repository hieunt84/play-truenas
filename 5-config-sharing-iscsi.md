
### Intro
    - config sharing iscsi.

### Config
    - create zvol from Pool 
      Goto: Storage > Pool > : > Zvol
   <p align="center"><img src="https://github.com/hieunt84/play-truenas/blob/master/images/config-add-zvol.PNG" /></p>

    - config sharing 
      Goto: Sharing > Block Share (iSCSI) > Wizard > ...
   <p align="center"><img src="https://github.com/hieunt84/play-truenas/blob/master/images/config-sharing-iscsi.PNG" /></p>

  
### Conclusion
    Result result-sharing-iscsi.PNG
   <p align="center"><img src="https://github.com/hieunt84/play-truenas/blob/master/images/result-sharing-iscsi.PNG" /></p>

### Expand volume iscsi
    Server Nas:
      Goto: Storage > Pool > Select iscsi-vol > : > Edit Zvol
    Client/Initator Window
      Goto: Disk management > Extend Volume
    Client/Initator Linux
      Goto: https://github.com/hieunt84/play-linux/blob/master/setup-new-disk/setup-new-disk-iscsi.md

### Ref
    [Ref].(https://www.youtube.com/watch?v=PBAMCifr1VY)    
