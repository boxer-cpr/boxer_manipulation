cmake_minimum_required(VERSION 2.8.3)
project(boxer_ur_description)

find_package(catkin REQUIRED)

catkin_package()

include_directories()

install(DIRECTORY urdf
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}
)
install(PROGRAMS
  scripts/setup_boxer_ur5_e_envar
  scripts/setup_boxer_ur5_envar
  DESTINATION ${CATKIN_PACKAGE_BIN_DESTINATION}
)
