cmake_minimum_required(VERSION 4.2)

# TODO: Rename project
project(Project LANGUAGES CXX)

add_executable(${PROJECT_NAME}
  src/main.cpp
)

# TODO: Add targets if needed
foreach(target ${PROJECT_NAME})
    set_target_properties(${target} PROPERTIES
        RUNTIME_OUTPUT_DIRECTORY_DEBUG ${CMAKE_SOURCE_DIR}/Output/Debug/${target}
        RUNTIME_OUTPUT_DIRECTORY_RELEASE ${CMAKE_SOURCE_DIR}/Output/Release/${target}
    )
endforeach()
