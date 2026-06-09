cmake_minimum_required(VERSION 3.25)

find_package(Geode REQUIRED)
project(AILevelEditor)

setup_geode_mod(com.myleveleditor.ai)

add_geode_mod(
    com.myleveleditor.ai
    SOURCES
        main.cpp
        text.cpp
)
