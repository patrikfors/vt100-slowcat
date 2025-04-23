cmake_minimum_required(VERSION 3.20)
project(slowcat LANGUAGES C CXX)

add_executable(slowcat)
target_sources(slowcat PRIVATE slowcat.cpp usleep.cpp getopt.c)
target_compile_features(slowcat PRIVATE cxx_std_20)

