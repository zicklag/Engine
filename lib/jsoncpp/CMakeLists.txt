if(MSVC)
	set(CMAKE_CXX_FLAGS_RELEASE "/MT /O2 /Ob2 /D NDEBUG")
endif()

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS_RELEASE} -fPIC" )

add_library(jsoncpp jsoncpp.cpp)
target_link_libraries(jsoncpp)
