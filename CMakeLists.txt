cmake_minimum_required(VERSION 3.8)
project(WickedAdventure)

add_subdirectory(WickedEngine)

set(SOURCE_FILES
    main_linux.cpp
)

add_executable(WickedAdventure ${SOURCE_FILES})

target_include_directories(WickedAdventure PUBLIC ${CMAKE_CURRENT_SOURCE_DIR}/WickedEngine/WickedEngine)

target_link_libraries(WickedAdventure PUBLIC WickedEngine)

