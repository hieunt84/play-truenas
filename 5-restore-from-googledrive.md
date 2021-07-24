
### Intro
    Restore dataset from google drive

### Config
    - Clone dataset from snapshot or make new dataset
    - Create Cloud Sync Task
      Goto: Tasks > Cloud Sync Tasks > ADD
        Source:/mnt/pool1/dataset-restore
        Destination:backup
        Direction: Pull
        Transfer Mode: Copy
        Schedule: None
    - Run Now
    
### Ref
    http://storagegaga.com/cloud-sync-prowess-of-freenas/
    https://www.truenas.com/docs/core/solutions/optimizations/disasterrecovery/
   