cmake_minimum_required(VERSION 2.8.3)
project(boxer_manipulation_description)
find_package(catkin REQUIRED)

catkin_package()

include_directories()

install(DIRECTORY meshes urdf
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}
)
install(PROGRAMS
  scripts/launch_delay.sh
  DESTINATION ${CATKIN_PACKAGE_BIN_DESTINATION}
)
