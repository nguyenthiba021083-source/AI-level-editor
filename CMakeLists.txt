cmake_minimum_required(VERSION 3.25)

status("Loading Geode Framework...")
find_package(Geode REQUIRED)

project(AILevelEditor)

setup_geode_mod(com.myleveleditor.ai)

add_geode_mod(
    com.myleveleditor.ai
    RESOURCES
    SOURCES
        src/main.cpp
)
