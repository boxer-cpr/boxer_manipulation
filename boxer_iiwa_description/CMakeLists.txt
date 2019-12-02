cmake_minimum_required(VERSION 2.8.3)
project(boxer_iiwa_description)
find_package(catkin REQUIRED)

catkin_package()

include_directories()

install(DIRECTORY urdf
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}
)
install(PROGRAMS
  scripts/setup_boxer_iiwa_7_envar
  DESTINATION ${CATKIN_PACKAGE_BIN_DESTINATION}
)
