cmake_minimum_required(VERSION 2.8.3)
project(my_randomgazebomanager_pkg)

## Compile as C++11, supported in ROS Kinetic and newer
# add_compile_options(-std=c++11)


find_package(catkin REQUIRED COMPONENTS
  gazebo_ros
  roscpp
  rospy
)


catkin_python_setup()


## Generate services in the 'srv' folder
add_service_files(
   FILES
   FetchMove.srv
 )


## Generate added messages and services with any dependencies listed here
generate_messages(
   DEPENDENCIES
   std_msgs
   geometry_msgs
 )


catkin_package(
  CATKIN_DEPENDS rospy
)


include_directories(
  ${catkin_INCLUDE_DIRS}
)


