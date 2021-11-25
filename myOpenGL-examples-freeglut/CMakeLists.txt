cmake_minimum_required(VERSION 3.0)

project(myOpenglSamples)

set(CMAKE_DISABLE_IN_SOURCE_BUILD ON)
set(CMAKE_SUPPRESS_REGENERATION ON)

include_directories(include/
                            freeglut/include/)
							
file(GLOB PROJECT_HEADERS include/*.h)
file(GLOB PROJECT_SOURCES src/*.cpp)
file(GLOB FREEGLUTLIBS freeglut/lib/freeglut.lib)	

source_group("Headers" FILES ${PROJECT_HEADERS})		
source_group("Sources" FILES ${PROJECT_SOURCES})	
source_group("FreeglutLib" FILES ${FREEGLUTLIBS})

add_executable(${PROJECT_NAME} ${PROJECT_HEADERS} ${PROJECT_SOURCES})

target_link_libraries(${PROJECT_NAME} ${FREEGLUTLIBS})

set_target_properties(${PROJECT_NAME} PROPERTIES
    RUNTIME_OUTPUT_DIRECTORY_DEBUG  ${CMAKE_BINARY_DIR}/Debug
    RUNTIME_OUTPUT_DIRECTORY_RELEASE  ${CMAKE_BINARY_DIR}/Release)

file(COPY  freeglut/lib/freeglut.dll  DESTINATION ./Debug)	
file(COPY  freeglut/lib/freeglut.dll  DESTINATION ./Release)
			