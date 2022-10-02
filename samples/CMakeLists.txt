project(samples LANGUAGES CXX)

find_package(glfw3 CONFIG REQUIRED)
find_package(imgui CONFIG REQUIRED)
find_package(glad CONFIG REQUIRED)

set (SAMPLE_SOURCE_FILES
	imgui_impl_glfw.cpp
	imgui_impl_opengl2.cpp
	main.cpp)

set (SAMPLE_HEADER_FILES
	imgui_impl_glfw.h
	imgui_impl_opengl2.h)

add_executable(samples ${SAMPLE_SOURCE_FILES} ${SAMPLE_HEADER_FILES})
target_include_directories(samples PRIVATE ${CMAKE_CURRENT_SOURCE_DIR})
target_link_libraries(samples PRIVATE box2d-lite glfw imgui::imgui glad::glad ${OPENGL_LIBRARIES})
