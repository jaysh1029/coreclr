cmake_minimum_required(VERSION 2.8.12.2)

set(CMAKE_INCLUDE_CURRENT_DIR ON)

set(SOURCES
  CreateFileMapping.c
)

add_executable(paltest_createfilemappinga_test6
  ${SOURCES}
)

add_dependencies(paltest_createfilemappinga_test6 CoreClrPal)

target_link_libraries(paltest_createfilemappinga_test6
  pthread
  rt
  m
  CoreClrPal
)
