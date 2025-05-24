## 本仓库仅供课程学习使用
## 智能工程实验：视觉ORB_SLAM3
### 编译：
- cd /home/robot/catkin_view/src/ORB_SLAM3/build
- rm -rf *
- cmake .. -DCMAKE_BUILD_TYPE=Release
- make -j$(nproc)

### 使用
- 检查连接：lsusb | grep RealSense
- 测试：realsense-viewer
- cd /home/robot/catkin_view/src/ORB_SLAM3/result
- 无IMU：../Examples/Stereo/stereo_realsense_D455 ../Vocabulary/ORBvoc.txt ../Examples/Stereo/RealSense_D455.yaml
- 无IMU，加载地图：../Examples/Stereo/stereo_realsense_D455 ../Vocabulary/ORBvoc.txt ../Examples/Stereo/RealSense_D455_load.yaml 
- cd /home/robot/catkin_view/src/ORB_SLAM3/result_IMU
- 有IMU：../Examples/Stereo-Inertial/stereo_inertial_realsense_D455 ../Vocabulary/ORBvoc.txt ../Examples/Stereo-Inertial/RealSense_D455.yaml
- 有IMU，加载地图：../Examples/Stereo-Inertial/stereo_inertial_realsense_D455 ../Vocabulary/ORBvoc.txt ../Examples/Stereo-Inertial/RealSense_D455_load.yaml
- 查看：pcl_viewer map.pcd

### 提交：
- 'src/ORB_SLAM3/Vocabulary/ORBvoc.txt'因过大未上传
