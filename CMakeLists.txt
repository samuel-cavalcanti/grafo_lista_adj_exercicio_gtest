cmake_minimum_required(VERSION 3.17)
project(grafo_lista_de_adjacencias)

set(CMAKE_CXX_STANDARD 11)

find_package(GTest REQUIRED)

set(HEADERS
        grafolistaadjexercicio.h
        )

set(SOURCES
        grafolistaadjexercicio.cpp
        )

set(TESTS
        grafoListaAdj.test.h
        )

add_executable(grafo_lista_de_adjacencias main.cpp ${HEADERS} ${SOURCES} )

add_executable(runUnitTests main.test.cpp ${HEADERS} ${SOURCES} ${TESTS} )

target_link_libraries(runUnitTests GTest::GTest GTest::Main)