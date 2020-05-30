project(hello)

add_executable(cpp main.cpp)

target_link_libraries(cpp PRIVATE say-hello)