cmake_minimum_required (VERSION 2.8)

set(ONEDRIVE_LIB_NAME "libonedrive")
set(FUSEMODULE_EXE_NAME "onedrive-client")
set(STANDALONE_NAME "ondrive-query")

set(LIB_VERSION_MAJOR 0)
set(LIB_VERSION_MINOR 1)

set(FUSEMODULE_VERSION_MAJOR 0)
set(FUSEMODULE_VERSION_MINOR 1)

set(STANDALONE_VERSION_MAJOR 0)
set(STANDALONE_VERSION_MINOR 1)

project (PROJECT_NAME)
include_directories("${PROJECT_SOURCE_DIR}/include")
set (LIBSRC ${PROJECT_SOURCE_DIR}/lib)
add_library(${PROJECT_NAME} "${LIBSRC}/onedrive.c")
