# Ardupilot Contributions

### [Cartographer: Added ceres_scan_matcher tuning parameters for multicopter](https://github.com/ArduPilot/ardupilot_wiki/pull/4303)
Fixed an issue where SLAM problems estimating position without remapping. Added remap tag with appropriate topics.

### [Cartographer:Updated Cartographer launch "Remap odom and imu data](https://github.com/ArduPilot/ardupilot_wiki/pull/4289)
Added ceresScanMatcher and realtimeCorrelativeScanMatching tuning parameters in cartographer.lua required to tune cartographer especially for multicopters

### [Plane: Updated highest airspeed limit when armed](https://github.com/ArduPilot/ardupilot/pull/20553)
Fixed an issue during takeoff of highest airspeed limit in cases like wind gusts causing takeoff rotation early

### [Copter: Remove glitch check for non-GNSS vehicle](https://github.com/ArduPilot/ardupilot/pull/20565)
Prevents unnecessary glitch check for non-GNSS copter

#
# GSOC project updates

### All the test related to Non-GPS Navigation and obstacle avoidance done on simulation

- Changes already mentioned in the proposal
- Rover was already working fine, so all the changes in parameters and code is done related to multicopter
- Multicopter, as of now, can hold/maintain its altitude even after giving 2D-nav-goals from RVIZ
- Some minor bugs in obstacle avaoidance but those are only for multicopter. For rover, it is working perfectly fine

### For integrating the offboard object avoidance with ArduPilot Auto mode

- Made changes according to Randy sir's pull on mavros code
- Used mavlink_router and replaced rviz by Mission planner
- Making changes mention by Voon to make a separate plugin (as already mentioned in my proposal)

#
# Non-Ardupilot contributions (related)

### [Extended object tracking using 2D LiDAR scans](https://github.com/snktshrma/obstacle_cluster_detection)
An obstacle detection module using 2D Lidar scans. The environment contains one or more moving objects. When objects are within the range of 2 meters, a ros message is published as an output containing: the number of obstacles, the distances to the obstacles and the sizes of obstacles.
