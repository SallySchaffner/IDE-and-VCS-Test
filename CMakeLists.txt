cmake_minimum_required(VERSION 3.16)

# Project name and language
project(MyProject LANGUAGES CXX)

# Set C++ standard (change to 17 or 20 if you prefer)
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

# Add the executable
add_executable(${PROJECT_NAME}
    src/main.cpp
)

# Add include directory (optional but common)
target_include_directories(${PROJECT_NAME}
    PRIVATE
        ${PROJECT_SOURCE_DIR}/include
)

