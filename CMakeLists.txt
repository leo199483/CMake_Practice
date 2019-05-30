    
cmake_minimum_required(VERSION 3.6)

# The project name
project(hello_cmake)

if(MSVC)
    #warning level 4 and all warnings as errors
    add_compile_options(/W4/WX)
else()
    #lots of warnings and all warnings as errors
    add_compile_options(-Wall -Wextra -pedantic -Werror)
endif()

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

