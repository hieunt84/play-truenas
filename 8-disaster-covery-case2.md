
### Intro
    Recovery after disaster

### Script
    truenas1 crashed
    ransomeware disaster

### Config recovery
    On Truenas1:
    - Build again truenas1
    - Create dataset same name with dataset on truenas2

    One Truenas2
    - Create Cloud Sync Task
      Goto: Tasks > Replication Tasks > ADD
        Source:/mnt/pool1/dataset1
        Destination:/mnt/pool1/dataset1
        Transfer Method: Pull
        Schedule: None
    - Run Now
    
### Ref  