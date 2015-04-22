cmake_minimum_required(VERSION 2.8)

include_directories( ../include)

# set source/lib variables
set(delegates_sources DelegateTests.cpp ../include/Delegate.h)
set(closure_sources ClosureTests.cpp ../include/closure.h)

# make project/target
project(delegates-tests CXX)
add_executable(DelegateTest ${delegates_sources})
add_executable(ClosureTest ${closure_sources})
