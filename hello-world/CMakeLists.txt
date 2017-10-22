# inspired by https://github.com/springkim/FSpring/blob/master/FSpring(ubuntu)/CMakeLists.txt
cmake_minimum_required(VERSION 3.8)
project(nanatest)


set(CMAKE_CXX_STANDARD 11)
set(SOURCE_FILES
    src/main.cpp
)

include_directories(/home/ale/bin/nana/include/)
link_directories(/home/ale/bin/nana/lib/)

add_executable(nanatest ${SOURCE_FILES})


target_link_libraries(nanatest nana X11 stdc++fs pthread fontconfig Xft)

