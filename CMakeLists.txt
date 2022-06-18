cmake_minimum_required(VERSION 2.8.9)

project(DatabaseInteractor)

set(DatabaseInteractor_VERSION_MAJOR 1)
set(DatabaseInteractor_VERSION_MINOR 1)
set(DatabaseInteractor_VERSION_PATCH 1)

#-----------------------------------------------------------------------------
# Extension meta-information
set(EXTENSION_HOMEPAGE "http://slicer.org/slicerWiki/index.php/Documentation/Nightly/Extensions/DatabaseInteractor")
set(EXTENSION_CATEGORY "Web System Tools")
set(EXTENSION_CONTRIBUTORS "Clement Mirabel (University of Michigan), Juan Carlos Prieto (UNC)")
set(EXTENSION_DESCRIPTION "This extension can interact with online data in a database and local folders.")
set(EXTENSION_ICONURL "https://raw.githubusercontent.com/DCBIA-OrthoLab/DatabaseInteractorExtension/master/DatabaseInteractor.png")
set(EXTENSION_SCREENSHOTURLS "https://raw.githubusercontent.com/DCBIA-OrthoLab/DatabaseInteractorExtension/master/FullView_DatabaseInteractor.png" "https://raw.githubusercontent.com/DCBIA-OrthoLab/DatabaseInteractorExtension/master/DatabaseInteractor_Interface.png")
set(EXTENSION_DEPENDS "NA") # Specified as a space separated string, a list or 'NA' if any

#-----------------------------------------------------------------------------
# Extension dependencies
find_package(Slicer REQUIRED)
include(${Slicer_USE_FILE})

#-----------------------------------------------------------------------------
# Extension modules
add_subdirectory(DatabaseInteractor)
## NEXT_MODULE

#-----------------------------------------------------------------------------
include(${Slicer_EXTENSION_CPACK})
