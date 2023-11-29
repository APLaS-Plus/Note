# Ros创建包基本流程
## 1. 创造工作空间
`mkdir -p ~__space_name__/src`  
`cd ~/__space_name__/src`  
`catkin_init_workspace`  
## 2. 编译工作空间
编译一定是在总目录里面进行的  
`cd ~/__space_name__`  
`catkin_make`
## 3. 设置环境变量
`source ~/devel/setup.bash`
### 检查环境变量
`echo $ROS_PACKAGE_PATH`  
## 4. 创建功能包
`cd ~/__space_name__/src`  
这一步的依赖项常见的有`std_msgs`，`roscpp`，`rospy`  
`catkin_create_pkg __pkg_name__ [depend1] [depend2] [depend3]`
## 5. 编译功能包
`cd ~/__space_name__`  
`catkin_make`  
`source ~/__space_name__/devel/steup.bash`
