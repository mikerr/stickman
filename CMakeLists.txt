cmake_minimum_required(VERSION 3.9)
# has to be before project
if(PICO_SDK_PATH)
          include(${32BLIT_DIR}/32blit-pico/pico_sdk_import.cmake)
    endif()
project (stickman)
find_package(32BLIT CONFIG REQUIRED $32BLIT_DIR)
blit_executable (stickman stickman.cpp)
blit_metadata (stickman metadata.yml)
