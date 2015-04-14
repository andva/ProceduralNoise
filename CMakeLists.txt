project(noise)
cmake_minimum_required(VERSION 2.8.6)

FILE(GLOB_RECURSE NOISE_H ${CMAKE_CURRENT_SOURCE_DIR}/*.h)
FILE(GLOB_RECURSE NOISE_CPP ${CMAKE_CURRENT_SOURCE_DIR}/*.c*)

set(noise-Source
	${NOISE_H}
	${NOISE_CPP}
	)

add_library(noise
			${noise-Source}
	)