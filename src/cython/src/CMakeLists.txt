# Define Shared Libraries (For use in other CMakeLists
add_library(rectangle SHARED rectangle.cpp)
add_library(eigen_ex SHARED eigen_ex.cpp)

# Set shared library output location
set_target_properties(rectangle PROPERTIES LIBRARY_OUTPUT_DIRECTORY ${CMAKE_SOURCE_DIR}/lib)
set_target_properties(eigen_ex PROPERTIES LIBRARY_OUTPUT_DIRECTORY ${CMAKE_SOURCE_DIR}/lib)

# Set library output name
set_target_properties(rectangle PROPERTIES OUTPUT_NAME rectangle${BUILD_POSTFIX})
set_target_properties(eigen_ex PROPERTIES OUTPUT_NAME eigen_ex${BUILD_POSTFIX})


