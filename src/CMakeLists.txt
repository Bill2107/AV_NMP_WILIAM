cmake_minimum_required(VERSION 3.8)
project(nmp)


enable_testing()

add_subdirectory(googletest)

set(Sources
	main.cpp
	)

add_library(nmp STATIC ${Sources})
add_subdirectory(tests)