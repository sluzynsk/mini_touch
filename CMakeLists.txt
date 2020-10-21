cmake_minimum_required(VERSION 3.16.0)
include($ENV{IDF_PATH}/tools/cmake/project.cmake)
set(EXTRA_COMPONENT_DIRS components/lv_port_esp32/components/lv_examples components/lv_port_esp32/components/lvgl components/lv_port_esp32/components/lvgl_esp32_drivers/lvgl_tft components/lv_port_esp32/components/lvgl_esp32_drivers/lvgl_touch components/lv_port_esp32/components/lvgl_esp32_drivers)
project(mini-touch)
