#week_1 
#build_system 
#cmake 

For building I use cmake
this is an example of how I will use cmake:

```cmake
project(game_executable)

add_executable(game_executable
    src/main.cpp
)

target_link_libraries(game_executable
    PUBLIC
    engine
)

target_include_directories(game_executable
    PRIVATE
    ${CMAKE_CURRENT_SOURCE_DIR}/include
    ${engine_SOURCE_DIR}/include
)
```
