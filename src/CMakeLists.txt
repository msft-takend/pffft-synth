# CMakeList.txt : CMake project for CMakeProject1, include source and define
# project specific logic here.
#

# Add source to this project's executable.
add_library(pffft-lib "pffft.c" "pffft.h" "pffft.hpp")

if (CMAKE_VERSION VERSION_GREATER 3.12)
  set_property(TARGET pffft-lib PROPERTY CXX_STANDARD 20)
endif()

# TODO: Add tests and install targets if needed.
