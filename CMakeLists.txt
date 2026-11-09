cmake_minimum_required(VERSION 3.10 FATAL_ERROR)
project(KymodynamicAudit)

# Locate the CERN ROOT package and define required components
find_package(ROOT REQUIRED COMPONENTS Core MathCore Matrix Hist)

# Include ROOT directories
include(${ROOT_USE_FILE})
include_directories(${CMAKE_CURRENT_SOURCE_DIR} ${ROOT_INCLUDE_DIRS})

# Create the executable
add_executable(bl05_audit bl05_kymodynamic_audit.cpp)

# Link the ROOT libraries to the executable
target_link_libraries(bl05_audit ${ROOT_LIBRARIES})