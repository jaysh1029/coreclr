cmake_minimum_required(VERSION 2.8.12.2)

set(CMAKE_INCLUDE_CURRENT_DIR ON)

set(SOURCES
  test16.c
)

add_executable(paltest_snprintf_test16
  ${SOURCES}
)

add_dependencies(paltest_snprintf_test16 CoreClrPal)

target_link_libraries(paltest_snprintf_test16
  pthread
  rt
  m
  CoreClrPal
)
