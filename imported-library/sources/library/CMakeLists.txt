cmake_minimum_required(VERSION 3.0)

set(NAME library)

add_library(${NAME} SHARED IMPORTED GLOBAL)
set_target_properties(${NAME} PROPERTIES INTERFACE_INCLUDE_DIRECTORIES "${PROJECT_SOURCE_DIR}/include")
set_target_properties(${NAME} PROPERTIES IMPORTED_LOCATION "${PROJECT_SOURCE_DIR}/binaries/library.dll")
set_target_properties(${NAME} PROPERTIES IMPORTED_IMPLIB "${PROJECT_SOURCE_DIR}/binaries/library.lib")
