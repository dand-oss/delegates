cmake_minimum_required(VERSION 2.8)
project(delegates CXX)

###############
# ASI default settings
list(APPEND CMAKE_MODULE_PATH "$ENV{ASI}/cmake/Modules")
include(asv_cmake_defaults)
asv_cmake_defaults( )
###############

add_subdirectory(tests)
#add_subdirectory(benchmarks)
add_subdirectory(src)

# includes
install(
    FILES include/closure.h  include/Delegate.h
    DESTINATION include/delegates
    )
