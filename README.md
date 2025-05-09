## 本仓库仅供课程学习使用
### 编译：
- cd /home/robot/catkin_view/src/ORB_SLAM3/build
- rm -rf *
- cmake .. -DCMAKE_BUILD_TYPE=Release
- make -j$(nproc)

### 使用
- cd /home/robot/catkin_view/src/ORB_SLAM3/result
- ../Examples/Stereo/stereo_realsense_D455 ../Vocabulary/ORBvoc.txt ../Examples/Stereo/RealSense_D455.yaml
- ../Examples/Stereo-Inertial/stereo_inertial_realsense_D455 ../Vocabulary/ORBvoc.txt ../Examples/Stereo-Inertial/RealSense_D455.yaml

### 提交：
- git -c http.proxy=http://127.0.0.1:7890 push -u origin master
- 'src/ORB_SLAM3/Vocabulary/ORBvoc.txt'因过大未上传