cmake_minimum_required(VERSION 2.8)

include_directories( ../include)

# set source/lib variables
set(delegates_sources delegateTests.cpp ../include/delegate.h)
set(closure_sources closureTests.cpp ../include/closure.h)

# make project/target
project(delegates-tests CXX)
add_executable(DelegateTest ${delegates_sources})
add_executable(ClosureTest ${closure_sources})

install(
    TARGETS DelegateTest ClosureTest
    DESTINATION bin
    )
