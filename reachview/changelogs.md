## ReachView changelog

### v2.5.0

###### Features

* New Correction input, output: bluetooth

### v2.4.0
([release](https://community.emlid.com/t/reachview-v2-4-0-galileo-support/5887/7))

###### Features

* Galileo support

###### Bug fixes

* Fixed a bug, which interfered with turning Glonass on or off
* Changed a notification message for Reach RS on low sat levels


### v2.3.1
([release](https://community.emlid.com/t/reachview-v2-3-1-point-collection/5855/8))

###### Bug fixes

* Fixed an issue with cache, which prevented the new Survey tab from opening immediately after the update


### v2.3.0
([release](https://community.emlid.com/t/reachview-v2-3-0-point-collection/5855/16))

###### Features

* Point collection support
* Collection screen with a realtime progress indicator, RTK and averaging statuses
* Collect the points either manually or with project-wide auto-save rules
* Project view with a map and summary point list
* Export your data to DXF, GeoJSON, Esri shapefiles


### v2.2.7
([release](https://community.emlid.com/t/reachview-v2-2-7/5523))

##### Features

* 3G/LTE USB modem support

##### Bug fixes

* Fixed an app crash, which happened if you turn off the base output configured to use LoRa
* Reworked USB-OTG on Reach RS. It didn't function properly on the pre-production units, but now those days are in the past


### v2.2.5 beta
([release](https://community.emlid.com/t/reachview-beta-v2-2-5/4988))

##### Bug fixes

* NTRIP issues fix
* Patch ERB to include correct geoid and ellipsoid heights


### v2.2.4 beta
([release](https://community.emlid.com/t/reachview-beta-v2-2-5/4988))

##### Features

* Update notifications


### v2.2.3 beta
([release](https://community.emlid.com/t/reachview-beta-v2-2-5/4988))

##### Bug fixes

* Fix bug of Reach crashing after a short period of work time


### v2.2.2 beta
([release](https://community.emlid.com/t/reachview-beta-v2-2-5/4988))

##### Bug fixes

* Fixed RTKLIB memory leak
* LoRa driver has got a heavy update
* Logs got a slight looks update and the whole tab will behave in a more stable fashion
* Fixed small frontend issues, like the LLH/XYZ selector placed poorly


### v2.2.1 beta
([release](https://community.emlid.com/t/reachview-beta-v2-2-5/4988))

##### Bug fixes

* The logs will not act insane when opening the logs tab
* Solution will not get lost
* The solution log will not restart for no apparent reason
* Solution format selector works as it is supposed to
* Merged RTCM3 fix by RtklibExplorer

### v2.2 beta
([release](https://community.emlid.com/t/reachview-beta-v2-2-5/4988))

##### Bug fixes
* Fixed wrong log split time
* Caching issues. While this is not a complete fix yet, this seriously improves the overall experience
* App prevented from crashing due to empty configuration files
* Increased timestamp precision in the solution output
* Solution log format mixup resolved
* Base coordinate reaveraging button is fixed

##### Features

* Reach RS support


### v2.1.6 beta
([release](https://community.emlid.com/t/reachview-beta-v2-1-6-is-out/4664))

##### Bug fixes
* Added units for the max acceleration settings
* Logging page reapplies logging settings


##### Features

* Added a special camera tab. Shows the time of the last received time mark and allows to setup Reach to trigger the camera automatically
* Added a button to delete logs from a whole day
* Automatically retrieve mountpoints available on an NTRIP service
* The solution log now has a selector, which lets you choose log format


### v2.1.5 beta

* Fix the bug with logs not saving their state after reboot

### v2.1.4 beta
([release](https://community.emlid.com/t/reachview-beta-v2-1-5-update/4544))

##### Bug fixes
* In-app connect to open wi-fi validation fails
* Loading screen disappears too early
* Logging: delete is glitchy with multiple files
* Satellite chart sorting: SBAS sats are separated from the rest
* Base sat levels are still displayed after corrections stop

##### Features

* RTKLIB update to newer beta. RTKLIB has been heavily updated
* Firefox support. Front-end has been updated to fix the insane behavior in this browser
* Display base on the map. 
* Smaller grid size. The minimum grid size has been decreased to 500mm

### v2.1.3 beta
([release](https://community.emlid.com/t/reachview-2-beta-v2-1-3-and-new-image/4495))

##### Bug fixes
* Disconnect not always working properly
* Make more informative disconnect notifications
* Implement NTRIP Server for base mode
* Display base on the map
* Base mode: add ability to average float
* Remember coordinate format after page refresh
* Fix a bug with map follow feature

##### Features

* New sattelite sorting

### v2.1.2 beta
([release](https://community.emlid.com/t/reachview-2-beta-v2-1-1/4404/49))

* Fixes Serial/USB problems


### v2.1.1 beta
([release](https://community.emlid.com/t/reachview-2-beta-v2-1-1/4404))

* Bug fixes
* Updater progress bar implemented
* Added loading screen

### v2.0 beta
([release](https://community.emlid.com/t/reachview-2-beta-release/4304))

* App rebuild. Improved general stability, user experience and usability. 

### v0.4.9

* Updated rtkrcv binary to RTKLIB 2.4.3 beta 16

### v0.4.8

* Fixed a bug with base not stopping correctly every time

### v0.4.7

* Updated RTKLIB binaries to 2.4.3 b16 and added a couple of patches by rtklibexplorer

### v0.4.6

* Updated **prnaccel** and **arlockcnt** values in default config files for better RTK results

### v0.4.5

* Added log delete confirmation popup
* Added button to delete logs by day
* Correction logs are now present in the logs tab

### v0.4.4

* Added RTKLIB integrity check on startup, which fixes the bug with logs not downloading properly
* Updated rtkrcv for better performance with dynamic filter on. 
* Updated rtkrcv send to more complete NMEA GGA to the base
* Improve startup time

### v0.4.3

* Updated repository readme

### v0.4.2

* Fixed lat-lon mix up in the status header

### v0.4.1

* Fixed a bug with two solutions set to file
* Fixed a bug with conversion cancellation
* JS console inside the app now shows full RTKLIB status

### v0.4.0

* Added support for UBX time marks when converting logs to RINEX

### v0.3.4

* Fixed an issue with Solution output 2 not working by itself

### v0.3.3

* Updated RINEX conversion timer to be more reailistic

### v0.3.2

* Added space meter to the logs tab
* RINEX logs now include SNR, doppler frequency and more
* Minimized probability of Reach forgetting its state

### v0.3.1

* Added Dynamic filter option to the rover's general tab.
* Fixed an issue where bluetooth.service file could be corrupted
* Added USB baud rate option

### v0.3.0

* Added ERB protocol support for Pixhawk integration

### v0.2.2

* Fixed not starting properly without an internet connection

### v0.2.1

* Fixed an issue where users with older ReachView version could not update correctly

### v0.2.0

* Added support for bluetooth scanning and pairing via ReachView
* Enabled bluetooth solution and log output

### v0.1.4

* Added Emlid favicon to the app

### v0.1.3

* ReachView will now show a blocking warning message when Reach is disconnected

### v0.1.2

* Added more headers to disable caching in browsers

### v0.1.1

* Set system time according to NTP(if available) or GPS on startup
* ReachView will start processing/logging until time is set

### v0.1.0

* Updated log tab looks
* Added reboot and turn off wi-fi buttons to settings tab
* Added image version to settings tab
* Added RINEX version chooser to settings tab
* Serial ports are now are now chosen from a select control
* Bugfixes

### v0.0.5

* Automatic log conversion to RINEX
* Fixed the issue, where base mode would not restart immediately
* Small visual updates and bugfixes

### v0.0.4

* Default receiver settings have been changed
* You can now set used GNSS systems and solution frequency for both base and rover modes
* Multiple bugfixes and improvements

### v0.0.3

* Moved the chart engine from [Chart.js](http://www.chartjs.org/) to [d3.js](http://d3js.org/)
* Added a separate "settings tab" with the update button and network information
* Pressing the update button now triggers an animation
* Minor visual updates to all tabs

### v0.0.2

* Fixed internal issue preventing the units from getting "<font color="yellow">Float</font>" or "<font color="green">Fix</font>" solution statuses in RTK modes

### v0.0.1

* First release


## Reach image changelog

### v2.1 beta
([release](https://community.emlid.com/t/reachview-2-beta-v2-1-3-and-new-image/4495))
([download link](https://files.emlid.com/images/ReachImage_v2.1_beta.zip))

* Intel's flashing tool issues solved



### v1.2

* Fixed the issue with unreliable Wi-Fi setup(mostly known as "Password does not match issue")
* Added various self-tests for corrupt internal software

### v1.1

* Fixed the issue preventing Reach from booting with a radio connected to a DF-13 connector
* Changes to boot setup process

### v1.0

* First release
