cmake_minimum_required(VERSION 2.8.9)

project(MyFirstSlicerExtension)

#-----------------------------------------------------------------------------
# Extension meta-information
set(EXTENSION_HOMEPAGE "https://github.com/tdougherty27/MyFirstSlicerExtension")
set(EXTENSION_CATEGORY "Learning")
set(EXTENSION_CONTRIBUTORS "Tim Dougherty (University of Iowa)")
set(EXTENSION_DESCRIPTION "This extension is developed as part of a tutorial")
set(EXTENSION_ICONURL "https://raw.github.com/tdougherty27/MyFirstSlicerExtension/master/MyFirstSlicerExtension.png")
set(EXTENSION_SCREENSHOTURLS "http://www.example.com/Slicer/Extensions/MyFirstSlicerExtension/Screenshots/1.png")

#-----------------------------------------------------------------------------
# Extension dependencies
find_package(Slicer REQUIRED)
include(${Slicer_USE_FILE})

#-----------------------------------------------------------------------------
# Extension modules
add_subdirectory(LineIntensityProfile)
## NEXT_MODULE

#-----------------------------------------------------------------------------
include(${Slicer_EXTENSION_CPACK})
