cmake_minimum_required(VERSION 3.16)

project(AILevelEditor)

include(FetchContent)

# GitHub tự động tải cấu hình Geode về máy chủ
FetchContent_Declare(
    Geode
    GIT_REPOSITORY https://github.com
    GIT_TAG        main
)
FetchContent_MakeAvailable(Geode)

# Thiết lập mod
setup_geode_mod(com.myleveleditor.ai)

add_geode_mod(
    com.myleveleditor.ai
    SOURCES
        main.cpp
        text.cpp
)
