# ConTi-Cal : Conic-based Thermal-infrared camera Calibration considering distortion parameter

ConTi-Cal is the fast and efficient conic based calibration method for thermal-infrared camera using the portable buttonhole shape target. 

The only thing we need to prepare for calibration is a moniter.

**The code will be released after the review session**

## How to run ConTi-Cal in ros?
  0. manufacture the calibration target using the stl file in target folder
  1. <a href="http://wiki.ros.org/melodic/Installation/Ubuntu">install ros</a> (melodic version is recommended) 
  2. <a href="http://ceres-solver.org/installation.html">install ceres solver</a> 
  3. make workspace and launch .launch file
  ```
  mkdir -p contical_ws/src
  cd contical_ws/src
  git clone https://github.com/ChaehyeonSong/ConTiCal/
  cd ..
  catkin_make
  source devel/setup.bash
  roslanch contical contical.launch
  ```
## Circle detection examples
