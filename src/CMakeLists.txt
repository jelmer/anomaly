cmake_minimum_required(VERSION 2.8)
include_directories (${CMAKE_SOURCE_DIR}/src
                     ${CMAKE_SOURCE_DIR}
                     ${ANOMALY_INCLUDE_DIRS})
add_executable(anomaly anomaly.cpp
                       Detector.cpp Detector.h)

install (TARGETS anomaly DESTINATION bin)

