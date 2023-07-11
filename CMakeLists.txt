# CMakeList.txt : CMake project for xmp, include source and define
# project specific logic here.
#

# Add source to this project's executable.
add_executable (xmp 
				xmp.cpp 
				)

if (CMAKE_VERSION VERSION_GREATER 3.12)
  set_property(TARGET xmp PROPERTY CXX_STANDARD 20)
endif()

# TODO: Add tests and install targets if needed.
target_include_directories(${PROJECT_NAME} PUBLIC ${INCLUDE_DIR})
target_link_libraries(${PROJECT_NAME}
${CMAKE_SOURCE_DIR}/lib/Debug/XMPCoreStatic.lib
${CMAKE_SOURCE_DIR}/lib/Debug/XMPFilesStatic.lib
# ${CMAKE_SOURCE_DIR}/lib/Release/XMPCoreStatic.lib
# ${CMAKE_SOURCE_DIR}/lib/Release/XMPFilesStatic.lib
)
