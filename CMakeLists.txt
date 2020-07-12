cmake_minimum_required(VERSION 3.16)
project(lvgl)

file(GLOB_RECURSE SOURCES "*.c")

set(LVGL_INCLUDE_DIRS ${PROJECT_SOURCE_DIR})
set(LVGL_LIBRARIES $<TARGET_FILE:lvgl>)

add_library(lvgl STATIC ${SOURCES})
