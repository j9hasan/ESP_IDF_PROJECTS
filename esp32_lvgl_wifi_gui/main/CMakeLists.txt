

set(SOURCES app_main.c )

idf_component_register(SRCS ${SOURCES}
                       INCLUDE_DIRS .
                       REQUIRES lvgl_esp32_drivers lvgl ui shared_task nvs_flash
                      )


target_compile_definitions(${COMPONENT_LIB} PRIVATE LV_CONF_INCLUDE_SIMPLE=1)



