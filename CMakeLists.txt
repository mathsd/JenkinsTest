cmake_minimum_required(VERSION 3.1)

Project(hello)

ADD_LIBRARY(hello STATIC hello.cpp)
ADD_EXECUTABLE(hi main.cpp)
TARGET_LINK_LIBRARIES(hi hello)

