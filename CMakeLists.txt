cmake_minimum_required (VERSION 2.6)
project (CasHMC)
set (CasHMC_VERSION_MAJOR 1)
set (CasHMC_VERSION_MINOR 0)

include_directories(sources)

add_definitions( -DDEBUG_LOG )

set (CXX_OPTIONS "-g -O3")

add_definitions( ${CXX_OPTIONS})

file(GLOB SOURCES "sources/*.cpp")

add_executable(CasHMC ${SOURCES})

