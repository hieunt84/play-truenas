
### Intro
    Disaster Recovery Solution

### Prepare
    - TrueNas2 for Disaster Recovery Solution

### Config
    Trên Truenas2:
    - Tạo dataset cùng tên với dataset cần replicate trên truenas1
    Trên Truenas1:
    - Create Cloud Sync Task
      Goto: Tasks > Replication Tasks > ADD
        Source:/mnt/pool1/dataset1
        Destination:/mnt/dataset1
        Schedule: None
    - Run Now
    
### Ref
    https://www.truenas.com/docs/core/solutions/optimizations/disasterrecovery/
    https://www.truenas.com/docs/core/tasks/replicationtasks/
   