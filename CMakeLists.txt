cmake_minimum_required(VERSION 3.20.0)

set(BOARD native_sim)
find_package(Zephyr REQUIRED HINTS $ENV{ZEPHYR_BASE})
project(level-meter)
file(GLOB SOURCES src/**/*.c src/*.c)
target_sources(app PRIVATE ${SOURCES})