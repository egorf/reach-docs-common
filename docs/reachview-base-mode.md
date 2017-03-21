## Base correction output
### Communication methods
#### Serial
#### NTRIP
#### TCP
#### LoRa Radio (RS only)

### RTCM3 messages
**Minimal required messages**
1002	GPS L1 observations	 @ 1 Hz
1006	ARP station coordinate  @ 0.1 Hz

**Optional messages for other GNSS systems**  

- 1010	GLONASS L1 observation
- 1107	SBAS	MSM
- 1117	QZSS	MSM
- 1127	BeiDou MSM

**Specific messages for not-typical applications**  

- 1008	Antenna type
- 1019	GPS Ephemeris
- 1020	GLONASS Ephemeris

The minimal subset that is required for RTK to function is 1002 for GPS observation and 1006 for base station position. Enabling more messages or higher rates requires higher bandwidth, so 

### Base position
### Antenna height offset



