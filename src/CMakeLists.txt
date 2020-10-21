FILE(GLOB_RECURSE app_sources ${CMAKE_SOURCE_DIR}/src/*.*)

idf_component_register(SRCS ${app_sources}
    INCLUDE_DIRS .
    REQUIRES lvgl_esp32_drivers lvgl lvgl_tft lvgl_touch nvs_flash)

target_compile_definitions(${COMPONENT_LIB} PRIVATE LV_CONF_INCLUDE_SIMPLE=1)
