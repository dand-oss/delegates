cmake_minimum_required(VERSION 2.8)

include_directories( include)
include_directories( include/nonius)
include_directories( ../include)

# set source/lib variables
set(bench_sources src/bench.cpp src/benchmark_worker.cpp ../include/Delegate.h include/benchmark_worker.h)

# make project/target
project(benchmarks CXX)
add_executable(bench ${bench_sources})
