    
cmake_minimum_required(VERSION 3.6)

# The project name
project(hello_cmake)

add_subdirectory(thirdparty/catch)
add_subdirectory(src)
add_subdirectory(test)

# The sources shared between the main program and the tests
#set(PROJECT_SOURCES hello.cpp hello.h)

# The main program
#add_executable(prog main.cpp ${PROJECT_SOURCES})

# The tests
#add_subdirectory(thirdparty/catch)
#add_executable(tests testmain.cpp ${PROJECT_SOURCES})
#target_include_directories(tests PRIVATE catch)

