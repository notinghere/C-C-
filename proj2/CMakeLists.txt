project(test2)

add_executable(${PROJECT_NAME} ./src/main.cpp)

target_include_directories(${PROJECT_NAME} PUBLIC ${ROOT_DIR}/include)
target_link_directories(${PROJECT_NAME} PUBLIC ${ROOT_DIR}/lib)
target_link_libraries(${PROJECT_NAME} PUBLIC hello_library)