
### Intro
    - Create Pool    
    - Config Raid
    - Raid Z is software raid

### Config
    1.yêu cầu ít nhất 3 disk giống nhau.
    2.Add pool
      Go to: Storage > Pool > Add > Creat new pool
   <p align="center"><img src="https://github.com/hieunt84/play-truenas/blob/master/images/add-pool.PNG" /></p>
 
    3.config pool
      - tùy thuộc số lượng đĩa sẽ có chiến lược cấu hình raid phù hợp.
      - config cache with 1 disk nvme 18GB.
      - config raidz1(raid5) with 3 disk 16GB.
   <p align="center"><img src="https://github.com/hieunt84/play-truenas/blob/master/images/config-pool.PNG" /></p>

    4.result-create-pool.PNG
   <p align="center"><img src="https://github.com/hieunt84/play-truenas/blob/master/images/result-create-pool.PNG" /></p>
  
### Conclusion
    Result create pool storage.
### Ref
    https://linuxhint.com/what_is_raidz/
    https://www.youtube.com/watch?v=-AnkHc7N0zM

   