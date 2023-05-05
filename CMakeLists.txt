cmake_minimum_required(VERSION 3.0.2)
project(test)



link_directories(
  /usr/local/lib 
  )
  

  
include_directories( include )

add_executable(testqjj  test.cpp  )

target_link_libraries(testqjj
                       libosqp.so  
                       libOsqpEigen.so 
                       libqdldl.so 
                       )
