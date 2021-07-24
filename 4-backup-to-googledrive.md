
### Intro
    Backup dataset from TrueNAS to google drive

### Config
    - Get ID Google Drive with rsync (optional)
    - Config Cloud Credentials for Google Drive
      Goto: System > Cloud Credentials > ADD >
        Provider: Google Drive
        Logging to Provider
        Verify
    - Make folder backup on Google Drive
    - Create Cloud Sync Task
      Goto: Tasks > Cloud Sync Tasks > ADD
        Source:/mnt/pool1/data
        Destination:backup
        Direction: Push
        Transfer Mode: Copy
        Schedule
    - Run Now
    
### Conclusion
    Result
   <p align="center"><img src="https://github.com/hieunt84/play-truenas/blob/master/images/result-backup-to-googledriver.PNG" /></p>

### Ref
    http://storagegaga.com/cloud-sync-prowess-of-freenas/
    https://www.truenas.com/docs/core/solutions/optimizations/disasterrecovery/
   