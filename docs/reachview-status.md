This is the main dashboard with all information about position and satellite reception.

## Satellite SNR chart

![](img/status/status.png)

RTK positioning requires excellent reception of signals from GNSS satellites. SNR (Signal to Noise Ratio) is the primary indicator of how good the reception is. The graph lists all satellites that fit in your screen size and corresponding SNR. Data is updated in real-time.

| Legend |                   |
|--------|-------------------|
|   R    | Glonass satellite |
|   G    | GPS satellite     |
|   S    | SBAS satellite    |
|   E    | Galileo satellite |
|   J    | QZSS satellite    |
|   B    | Beidou satellite  |
 

When SNR of a satellite is over 45, it will be marked green. Grey bars indicate SNR of the base station. You should aim to achieve as many satellites signals in “green zone” as possible. That will make your measurements precise and ambiguity resolution (Fix) fast. On the top of the SNR chart you can see indicators of numbers of satellites visible to rover and base receivers.

## RTK parameters

![](img/status/rtk_parameters.png)

### Age of differential
In case of steady correction steam age of differential will indicate link latency. Calculated by subtracting time when the correction message has been generated from the current receiver time. It is an invaluable tool to debug connectivity issues.

### AR validation ratio  
This is result of ratio test performed on the potential “Fix” solution, it shows how many times is the best solution better than the next one. If this number is more than 3 Reach will consider RTK solution Fixed. 

### Baseline
Baseline is the distance from rover to the base. It should be kept within 10km, if it is increased further you might experience slower fix time and lower accuracy. Accuracy is decreased by 1mm each km of baseline. 
 
## Map
Integrated map is used to show your current position. Map layer is provided by OpenStreetMap.

![](img/status/map.png)

Available map features:

+ Last point: zooms the map to the last point.
+ Clear map: deleted all current points on the map.
+ Hide background: removes OSM layer.
+ Follow: keeps focus on the last point.
+ Select number of points to show 100, 1000,10000.




| Point colors meaning |             |
|----------------------|-------------|
|        Green         |   RTK Fix   |
|        Yellow        |   RTK Float |
|        Red           |   Single    |


### Position
WGS84 Latitude and Longitude as well as ellipsoidal height are displayed on the status tab. Position display format can be changed to XYZ ECEF.

![](img/status/position.png)

### Solution status
"-" means there is no information for the software to process. Either not enough time has passed or the antenna is not placed correctly.  
Single means that rover has found a solution relying on it's own receiver and base corrections are not applied. Configuring positioning mode to Single will also result in this status. Precision in standalone mode is on meters-level.
Float means that base corrections are now taken into consideration and positioning is relative to base coordinates, but the integer ambiguity is not resolved. Precision in float mode is submeter-level.  
Fix means that positioning is relative to the base and the integer ambiguity is resolved. Precision in standalone mode is centimeter-level.


