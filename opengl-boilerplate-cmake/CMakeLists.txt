cmake_minimum_required (VERSION 3.8)

find_package(GLUT REQUIRED)
find_package(GLEW REQUIRED)
find_package(GLM REQUIRED)

add_executable (main "main.cpp")
target_include_directories(main PUBLIC ${GLUT_INCLUDE_DIR} ${GLEW_INCLUDE_DIR} ${GLM_INCLUDE_DIR})
target_link_libraries(main ${GLUT_LIBRARIES} ${GLEW_LIBRARIES} ${GLM_LIBARIES})
