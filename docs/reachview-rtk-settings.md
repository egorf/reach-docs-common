### RTK options
**Positioning mode**  

+ Single - standalone positioning mode, does not provide improved precision.
+ Kinematic - most used positioning mode, assumes that receiver is moving.
+ Static - an assumption is made that Reach is static. Constraining the system helps to resolve ambiguities faster as well as produce measurements with higher precision.
AR (Ambiguity resolution) mode
There are two main strategies for resolving ambiguities: 
Fix-and-hold: after first ambiguity fix hold them constrained. Fix is more stable

### GNSS selection

Depending on your location it might be beneficial to choose certain GNSS systems: 

+ GPS+Glonass+SBAS+QZSS at 5 Hz is our default recommendation
+ GPS+Beidou+SBAS+QZSS at 5 Hz recommended for APAC, where QZSS is visible
+ GPS+SBAS+QZSS at 14 Hz for most dynamic platforms that require high update rate




