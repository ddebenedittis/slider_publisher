cmake_minimum_required(VERSION 3.5)
project(slider_publisher)

find_package(ament_cmake REQUIRED)

install(DIRECTORY config launch
        DESTINATION share/${PROJECT_NAME})

install(PROGRAMS src/slider_publisher.py
        DESTINATION lib/${PROJECT_NAME})

ament_package()
