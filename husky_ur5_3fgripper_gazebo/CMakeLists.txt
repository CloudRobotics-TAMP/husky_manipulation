cmake_minimum_required(VERSION 2.8.3)
project(husky_ur5_3fgripper_gazebo)

find_package(catkin REQUIRED COMPONENTS roslaunch)

catkin_package()

roslaunch_add_file_check(launch)

catkin_install_python(PROGRAMS scripts/stow_ur5 scripts/open_3fgripper scripts/close_3fgripper DESTINATION ${CATKIN_PACKAGE_BIN_DESTINATION})

install(DIRECTORY config launch scripts
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}
)
