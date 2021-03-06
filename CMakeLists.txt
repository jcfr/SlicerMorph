cmake_minimum_required(VERSION 3.5)

project(SlicerMorph)

#-----------------------------------------------------------------------------
# Extension meta-information
set(EXTENSION_HOMEPAGE "http://slicer.org/slicerWiki/index.php/Documentation/Nightly/Extensions/SlicerMorph")
set(EXTENSION_CATEGORY "SlicerMorph")
set(EXTENSION_CONTRIBUTORS "Sara Rolfe (UW), Murat Maga (SCRI)")
set(EXTENSION_DESCRIPTION "This extension will load modules developed for the SlicerMorph project. ")
set(EXTENSION_ICONURL "SlicerMorph_Color.png")
set(EXTENSION_SCREENSHOTURLS "http://www.example.com/Slicer/Extensions/SlicerMorph/Screenshots/1.png")
set(EXTENSION_DEPENDS "NA") # Specified as a space separated string, a list or 'NA' if any

#-----------------------------------------------------------------------------
# Extension dependencies
find_package(Slicer REQUIRED)
include(${Slicer_USE_FILE})

#-----------------------------------------------------------------------------
# Extension modules
add_subdirectory(ConvertMorphologikaLandmarks)
add_subdirectory(GPA)
add_subdirectory(ImportSurfaceToSegment)
add_subdirectory(ReadLandmarkFile)
add_subdirectory(SkyscanReconImport)
add_subdirectory(MorphoSource)

## NEXT_MODULE

#-----------------------------------------------------------------------------
include(${Slicer_EXTENSION_GENERATE_CONFIG})
include(${Slicer_EXTENSION_CPACK})
