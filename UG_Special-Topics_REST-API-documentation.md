In Preferences you can enable a restful web service api that will be available whilst GC is running.
This provides URLs that you can call from Matlab, R et al to retrieve data. You can also access
these URLs using a standard browser too.

Data is made available for all athletes regardless of who GC is currently working with (i.e. which
athlete you selected). Alternatively, you can start GoldenCheetah with the command line option --server
and it will run as a service without a GUI. 

**SUPPORTED ENDPOINTS**

```
http://localhost:12021              
```
Default base URL

```
/                                   
```
List Athletes
* Returns csv of athletes and core data (dob, sex etc)

```
/<athlete>                          
```
List Athlete Rides with Metrics and Metadata
* since=yyyy/mm/dd 
* before=yyyy/mm/dd
* metrics=NP,IF,TSS,AveragePower
* metadata=none or all or list (Sport,Workout Code)
* intervals=true
* Returns csv of activities incl. metrics and metadata

```
/<athlete>/zones                    
```
List Athlete Zone Config
* for=xxx where xxx is one of power, hr, pace, swimpace
* Returns csv of zone config history (e.g. configured CP/W')

```
/<athlete>/activity/<filename>      
```
Fetch activity file
* format=xxx where xxx is one of csv, tcx, json, pwx
* Returns ride file data in the requested format

```
/<athlete>/meanmax/<filename>       
```
Fetch activity Mean Max data
* series=xxx where xxx is one of watts,hr,cad,speed,nm,vam.xPower,NP
* Returns csv of the mean max data for a ride

```
/<athlete>/meanmax/bests            
```
Fetch Mean Max Bests for a Date Range
* since=yyyy/mm/dd
* before=yyyy/mm/dd
* series=xxx where xxx is one of watts,hr,cad,speed,nm,vam.xPower,NP
* Returns an aggregate of the best mean maximal values over the date range