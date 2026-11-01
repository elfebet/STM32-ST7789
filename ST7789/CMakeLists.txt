file(GLOB ST7789_SOURCES "*.c" "adafruit_fonts/*.c")

target_sources(${CMAKE_PROJECT_NAME} PRIVATE ${ST7789_SOURCES})

target_include_directories(${CMAKE_PROJECT_NAME} PRIVATE
    ${CMAKE_CURRENT_SOURCE_DIR}
    ${CMAKE_CURRENT_SOURCE_DIR}/adafruit_fonts
)
