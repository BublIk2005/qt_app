cmake_minimum_required(VERSION 3.10)

project(qt_app)



include_directories(edge graphwidget main mainwindow moc node)
add_subdirectory(edge)
add_subdirectory(graphwidget)
add_subdirectory(main)
add_subdirectory(mainwindow)
add_subdirectory(node)
