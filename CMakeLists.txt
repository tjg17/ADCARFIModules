cmake_minimum_required(VERSION 2.8.9)

project(ADCARFIModules)

#-----------------------------------------------------------------------------
# Extension meta-information
set(EXTENSION_HOMEPAGE "http://www.example.com/Slicer/Extensions/ADCARFIModules")
set(EXTENSION_CATEGORY "Examples")
set(EXTENSION_CONTRIBUTORS "Tyler Glass (Nightingale Lab)")
set(EXTENSION_DESCRIPTION "This extension hosts custom modules for ADC and ARFI analysis.")
set(EXTENSION_ICONURL "http://www.example.com/Slicer/Extensions/ADCARFIModules.png")
set(EXTENSION_SCREENSHOTURLS "http://www.example.com/Slicer/Extensions/ADCARFIModules/Screenshots/1.png")

#-----------------------------------------------------------------------------
# Extension dependencies
find_package(Slicer REQUIRED)
include(${Slicer_USE_FILE})

#-----------------------------------------------------------------------------
# Extension modules
add_subdirectory(HistoStat)
## NEXT_MODULE

#-----------------------------------------------------------------------------
include(${Slicer_EXTENSION_CPACK})
