cmake_minimum_required(VERSION 2.8)

#test
PROJECT(demo)

INCLUDE_DIRECTORIES(
    ./include
)

AUX_SOURCE_DIRECTORY(src DIR_SRCS)

add_compile_options(-std=c++11)

SET(SRC ${DIR_SRCS})

LINK_DIRECTORIES(
    ./libs
)

ADD_EXECUTABLE(${PROJECT_NAME} ${SRC})

TARGET_LINK_LIBRARIES(${PROJECT_NAME} )
