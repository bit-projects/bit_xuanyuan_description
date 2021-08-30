
cmake_minimum_required(VERSION 3.1)

project(bit_xuanyuan_description VERSION 1.0.0)

find_package(catkin REQUIRED)

catkin_package()

foreach(dir meshes urdf)
  install(DIRECTORY ${dir}/
    DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}/${dir})
endforeach(dir)
