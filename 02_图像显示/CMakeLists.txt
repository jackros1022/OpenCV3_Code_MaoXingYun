cmake_minimum_required (VERSION 2.8)
project (ShowImage)

find_package( OpenCV REQUIRED )
include_directories( ${OpenCV_INCLUDE_DIRS} )

# add the executable
add_executable (2_ShowImage 2_ShowImage.cpp)
# target_link_libraries(2_ShowImage opencv_core opencv_highgui opencv_imgcodecs)
target_link_libraries(2_ShowImage ${OpenCV_LIBRARIES})