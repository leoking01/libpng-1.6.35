project(TestInstallation)
cmake_minimum_required(VERSION 3.5)

find_package(png 1.0  PATHS  "E:\\AAA_z\\libpng__install")

add_executable(mymathApp mymathApp.cc)
target_link_libraries(mymathApp  -lpng)
target_include_directories(mymathApp  PRIVATE  "E:\\AAA_z\\libpng__install/include")
