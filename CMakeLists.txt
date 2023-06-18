cmake_minimum_required(VERSION 3.0.0)
project(dcm2img VERSION 0.1.0 LANGUAGES C CXX)


add_executable(dcm2img dcm2img.cc djcodecd.cc djcparam.cc djdecode.cc djutils.cc memory_file.cpp)

set(CPACK_PROJECT_NAME ${PROJECT_NAME})
set(CPACK_PROJECT_VERSION ${PROJECT_VERSION})
include(CPack)

target_link_libraries(dcm2img dcmpstat dcmqrdb dcmtls dcmwlm dcmsr dcmnet dcmimage dcmjpls dcmrt dcmjpeg dcmimgle dcmiod dcmdata oflog ofstd oficonv ijg8 ijg12 ijg16 openjp2 dcmtkcharls z pthread)