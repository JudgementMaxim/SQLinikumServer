cmake_minimum_required(VERSION 3.31)
project(SQLinikumServer)

set(CMAKE_CXX_STANDARD 20)

add_executable(SQLinikumServer main.cpp
        src/Server.cpp
        include/Server.h
        src/ClientHandler.cpp
        include/ClientHandler.h
        src/DatabaseManager.cpp
        include/DatabaseManager.h
        src/Utils.cpp
        include/Utils.h)
