cmake_minimum_required(VERSION 3.10)
project(QrGen VERSION 0.1.0 LANGUAGES C CXX)

include(CTest)
enable_testing()

# find_package(GLEW REQUIRED)
# include_directories(${GLEW_INCLUDE_DIRS})
# link_libraries(${GLEW_LIBRARIES})

# find_package(SDL2 REQUIRED)
# include_directories(${SDL2_INCLUDE_DIRS})
# link_libraries(${SDL2_LIBRARIES})

add_executable(QrGen qrgen.cpp qrcodegen.cpp qrcodegen.hpp)
# target_link_libraries(Game GL)

set_property(TARGET QrGen PROPERTY CXX_STANDARD 23)
