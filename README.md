**Analyze Massachusetts Bay Transportation Authority(MBTA) Transit Data**   

*Description*   
-Deployed MySQL Server using Docker   
-Created database, table & inserted records into table by pulling data directly from MBTA API   
-Cleaned transit data using python to make it suitable for analysis   
-Analyzed & created visual representation of data to enable users & decision maker understand on the average time taken by each bus to complete the route 1 & provide them  an estimate of the speed of the bus from current_stop_sequence = 1 to the last current_stop_sequence to see performance of each bus   

*Assumptions*  
-Only considered data for buses which has completed route 1 (i.e. stop 1 to 24)  

*Findings*  
*1. Average time taken by bus*  
Bus_id y1869  
   -Bus_id y1869(with the maximum number of records in dataset) took on an average 41.94 minutes on 18 trips for completing route 1 (assuming start stop is 1 & end stop is 24)  
   -Time taken by bus_id y1869 to complete route 1 varies at different time with lowest at 11am(i.e. time taken is 23 minutes) & highest at 8pm(i.e. time taken is 65 minutes)   
   -Traffic starting at 11:18 am takes less time (22 min) compared to bus starting between 10am-10:40am. This is due to the fact that office traffic reduce after 11am  
   -Bus starting in morning takes less time compared to evening. Factors affecting traffic flow is commuters, office traffic, dinning, grocery shopping etc.  

All other buses   
   -On an average it takes around 40 to 50 minutes for a bus to complete route 1. Bus_id'y1873' took lowest 23 minutes & bus_id'y1863' took highest 67 minutes on an average
   -This can be due to number of factors:   
       a. Bus timings i.e. y1863 running only at peak traffic hours & y1873 running at low traffic hours   
       b. Speed of the bus     
       c. Weather conditions or any accidents       
       d. Any special events(such as concert) which may contribute in increased timings for buses  

*2. Speed of the bus from stop 1 to 24*   
-Speed of each bus varies with lowest speed at 6.8 km/hr for bus_id'y1736' & highest at 14.6 km/hr for bus_id'y1873'   


