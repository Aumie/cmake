project(say-hello) #sub proj name

add_library(
        say-hello
        src/say-hello/hello.h
        src/say-hello/hello.cpp
)

target_include_directories(say-hello PUBLIC "${CMAKE_CURRENT_SOURCE_DIR}/src")

target_compile_definitions(say-hello PUBLIC SAY_HELLO_VERSION=1)
#PRIVATE will be used only in lib
#INTERFACE outside lib