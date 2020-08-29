cmake_minimum_required(VERSION  3.10  FATAL_ERROR)

set(PROJECT_NAME BatleCity)

project(${PROJECT_NAME})

#set(CMAKE_CXX_STANDARD 17)
#set(CMAKE_CXX_STANDARD 20)


add_executable(${PROJECT_NAME}  src/main.cpp)

#target_link_libraries(${PROJECT_NAME} -lglut  -lGLU  -lGL)
#target_link_libraries(${PROJECT_NAME} -lGL -lglut -lGLEW)
#target_link_libraries(${PROJECT_NAME} #[[-lglfw3]] -lGL -lX11 -lpthread -lXrandr -lXi -ldl)
#target_link_libraries(${PROJECT_NAME} GL GLU glfw3 X11 Xxf86vm Xrandr pthread Xi dl Xinerama Xcursor assimp)
target_link_libraries(${PROJECT_NAME}  -lglfw3 -lGL -lm -lXrandr -lXi -lX11 -lXxf86vm -lpthread -ldl -lXinerama -lXcursor)
