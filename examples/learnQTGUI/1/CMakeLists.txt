# Generated from rasterwindow.pro.

cmake_minimum_required(VERSION 3.16)
project(learnQTGUI_1_raseterwindow LANGUAGES CXX)

set(CMAKE_INCLUDE_CURRENT_DIR ON)

set(CMAKE_AUTOMOC ON)
set(CMAKE_AUTORCC ON)
set(CMAKE_AUTOUIC ON)


# 添加应用                                    
qt_add_executable(${PROJECT_NAME}
    main.cpp
    rasterwindow.h
    rasterwindow.cpp
)

set_target_properties(${PROJECT_NAME} PROPERTIES
    WIN32_EXECUTABLE TRUE
    MACOSX_BUNDLE TRUE
)

# 链接库文件
target_link_libraries(${PROJECT_NAME} PUBLIC
    Qt::Core
    Qt::Gui
)
