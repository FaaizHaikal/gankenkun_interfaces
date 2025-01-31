cmake_minimum_required(VERSION 3.5)
project(gankenkun_interfaces)

find_package(ament_cmake REQUIRED)
find_package(rosidl_default_generators REQUIRED)

rosidl_generate_interfaces(gankenkun_interfaces
  "msg/Point2.msg"
  "msg/SetWalking.msg"
  "msg/Status.msg"
  "srv/GetConfig.srv"
  "srv/UpdateConfig.srv")

ament_export_dependencies(rosidl_default_runtime)
ament_package()
