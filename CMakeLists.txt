cmake_minimum_required(VERSION 2.8)	 
										
project(hello_world)			

set(SOURCE_EXE main.cpp)		

set(SOURCE_LIB calculator.cpp)			

set(SOURCE_LIB hello.cpp)

add_library(
	hello 
	STATIC 
	hello.cpp
)	

add_executable(
	main 
	main.cpp
)	

target_link_libraries(main hello)		
