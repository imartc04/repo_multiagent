cmake_minimum_required(VERSION 3.5)

project(prac4)

find_package(ament_cmake REQUIRED)
ament_package()

install(DIRECTORY
  config dashboard launch maps rviz 
  DESTINATION share/${PROJECT_NAME}/
)

add_custom_target(build ALL DEPENDS ${outputs})
