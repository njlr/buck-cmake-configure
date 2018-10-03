cmake_minimum_required(VERSION 3.12)

message(STATUS "CXX compiler ID: '${CMAKE_CXX_COMPILER_ID}'")
message(STATUS "CXX compiler Version: '${CMAKE_CXX_COMPILER_VERSION}'")

# Some variables we can use in the project 
# Could be anything 
set(VERSION_MAJOR 1)
set(VERSION_MINOR 2)
set(VERSION_PATCH 3)

# Require lambda functions 
set(CCF_REQUIRED_FEATURES
  cxx_lambdas
  cxx_constexpr
)

configure_file(
  config.h.in
  config.h
)
