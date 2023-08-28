# from path/Main/Source/CMakeLists.txt

# Settings :
include_directories(${CMAKE_SOURCE_DIR}/Main/Header)

# Files
file(GLOB_RECURSE ENGINE_SOURCES *.cpp *.c)
file(GLOB_RECURSE ENGINE_HEADERS *.hpp *.h *.inl)
add_executable(Main ${ENGINE_SOURCES} ${ENGINE_HEADERS})
target_link_libraries(Main glfw3 glew32)