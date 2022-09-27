project(hello_library)

#Generate the static library from the library sources
add_library(${PROJECT_NAME} STATIC src/Hello.cpp src/Hello.h)

install(DIRECTORY "${CMAKE_CURRENT_SOURCE_DIR}/src/"
        DESTINATION "${ROOT_DIR}/include/proj1"
        FILES_MATCHING
        PATTERN "*.hpp"
        PATTERN "*.h")