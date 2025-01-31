cmake_minimum_required(VERSION 3.5)
project(kansei_interfaces)

find_package(ament_cmake REQUIRED)
find_package(rosidl_default_generators REQUIRED)

rosidl_generate_interfaces(kansei_interfaces
  "msg/Point2.msg"
  "msg/SetWalking.msg"
  "msg/Status.msg"
  "srv/GetConfig.srv"
  "srv/UpdateConfig.srv")

ament_export_dependencies(rosidl_default_runtime)
ament_package()
