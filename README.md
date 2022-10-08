# ConTi-Cal : Conic-based Thermal-infrared camera Calibration considering distortion parameter

ConTi-Cal is the fast and efficient conic based calibration method for thermal-infrared camera using the portable buttonhole shape target. 

The only thing we need to prepare for calibration is a moniter.

**The code will be released after the review session**

## Abstract
Intrinsic calibration is an essential phase in uti-
lizing imaging sensor geometry. Unfortunately, traditional cal-
ibration necessitates a sophisticated procedure when applied
to thermal infrared (TIR) cameras. Furthermore, inherent
blunt and obscure thermal imaging boundaries hinder precise
detection, causing low calibration accuracy. To tackle these
challenges, we propose a novel approach to thermal camera
calibration exploitation based on conic. Existing conic-based
methods are limited to intrinsic parameter estimation because
conic does not hold the property under distortion. To mitigate
this issue, we introduce undistorted conic reconstruction for
reliable projection among thermal images and complete conic-
based optimization for distortion coefficient inference. We
further propose scale-invariant geometric losses, which are
robust to the inherent thermal image problems in that they
prevent severe image noise and pixel inaccuracy. As a result, our
method outperforms the ROS-calibrator, demonstrating about
10% error reduction.

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
## Demonstration
![12s](https://user-images.githubusercontent.com/106569301/194704702-db19ea73-7ec0-4402-9823-36763c5ce042.gif)

