cmake_minimum_required(VERSION 3.10)

project(qt_app)

set(CMAKE_AUTOMOC ON)
set(CMAKE_AUTORCC ON)
set(CMAKE_AUTOUIC ON)

#set(CMAKE_INCLUDE_CURRENT_DIR ON)
#set(CMAKE_INCLUDE_CURRENT_BINARY_DIR ON)

find_package(Qt5 COMPONENTS Core Gui Widgets REQUIRED)

#set(SRC_FILES qt_minimal_app.cpp)

#if (WIN32)
 # add_executable(qt_minimal_app WIN32 ${SRC_FILES})
#else()
  #add_executable(qt_minimal_app ${SRC_FILES})
#endif()
#target_link_libraries(qt_minimal_app Qt5::Widgets)


include_directories(edge graphwidget main mainwindow moc node)
add_subdirectory(edge)
add_subdirectory(graphwidget)
add_subdirectory(main)
add_subdirectory(mainwindow)
add_subdirectory(node)
