cmake_minimum_required( VERSION 3.16 )

list( APPEND CMAKE_MODULE_PATH ${CMAKE_SOURCE_DIR}/cmake )
include( common )

project( DISP CXX ) #set variable BACKEND_SOURCE_DIR
#project command must be before include directives

include( libs )

add_subdirectory( base )
add_subdirectory( NetLib )
add_subdirectory(api-gateway)
add_subdirectory(cars-service)
add_subdirectory(rental-service)
add_subdirectory(payments-service)
