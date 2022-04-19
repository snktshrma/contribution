# contributions

### [Plane: Updated highest airspeed limit when armed](https://github.com/ArduPilot/ardupilot/pull/20553)
Fixed an issue during takeoff of highest airspeed limit in cases like wind gusts causing takeoff rotation early

### [Cartographer: Added ceres_scan_matcher tuning parameters for multicopter](https://github.com/ArduPilot/ardupilot_wiki/pull/4303)
Fixed an issue where SLAM problems estimating position without remapping. Added remap tag with appropriate topics.

### [Cartographer:Updated Cartographer launch "Remap odom and imu data](https://github.com/ArduPilot/ardupilot_wiki/pull/4289)
Added ceresScanMatcher and realtimeCorrelativeScanMatching tuning parameters in cartographer.lua required to tune cartographer especially for multicopters

### [Copter: Remove glitch check for non-GNSS vehicle](https://github.com/ArduPilot/ardupilot/pull/20565)
Prevents unnecessary glitch check for non-GNSS copter
