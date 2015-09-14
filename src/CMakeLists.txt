cmake_minimum_required(VERSION 2.8)

include_directories( ../include)

# set source/lib variables
set(quickstart_sources quickstart.cpp ../include/delegate.h)

# make project/target
project(quickstart CXX)
add_executable(quickstart ${quickstart_sources})
