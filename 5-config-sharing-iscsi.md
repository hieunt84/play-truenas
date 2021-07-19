
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
      https://www.golinuxcloud.com/configure-iscsi-target-initiator-targetcli-rhel-centos-7/

### command to using iscsi disk on linux
    # add disk iscsi
    iscsiadm --mode discovery \
    --type sendtargets \
    --portal 172.20.10.110 \
    --discover 172.20.10.110:3260

    iscsiadm --mode node \
    --targetname iqn.2005-10.org.freenas.ctl:iscsi-linux \
    --login
   
    # Check new disk in system
    lsblk
    lsscis

    # partion disk
    fdisk -l
    fdisk /dev/sdb

    # format command
    mkfs.ext4 /dev/sdc1
    
    # mount
      mkdir -p /mnt/iscsi-vol
      vi /etc/fstab
        UUID=d1982789-cc22-4b8a-a9b8-612411b01526 /mnt/iscsi-vol     ext4   defaults        0 0
      mount /mnt/iscsi-vol

    # check mount 
    df-h or lsblk -f

### Ref
    https://www.youtube.com/watch?v=PBAMCifr1VY    
