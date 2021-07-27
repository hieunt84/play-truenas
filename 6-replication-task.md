
### Intro
    Disaster Recovery Solution
   
   <p align="center"><img src="https://github.com/hieunt84/play-truenas/blob/master/images/ cross-site-disaster-recovery.PNG" /></p>

### Prepare
    - TrueNas2 for Disaster Recovery Solution
    - on truenas1: create snaphost (manual or automatically) for dataset need replication.

### Config
    On Truenas2:
    - Create dataset same name with dataset on truenas1

    On Truenas1:
    - Create Cloud Sync Task
      Goto: Tasks > Replication Tasks > ADD
        Source:/mnt/pool1/dataset1
        Destination:/mnt/pool1/dataset1
        Schedule: None
    - Run Now
    
### Ref
    https://www.truenas.com/docs/core/solutions/optimizations/disasterrecovery/
    https://www.truenas.com/docs/core/tasks/replicationtasks/
    https://www.youtube.com/watch?v=J9pHMSaHhiI
   