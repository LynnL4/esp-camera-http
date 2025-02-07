file(GLOB app_sources ${CMAKE_CURRENT_SOURCE_DIR}/*.c)
idf_component_register(SRCS ${app_sources}
                        PRIV_INCLUDE_DIRS .
                        PRIV_REQUIRES nvs_flash esp_psram driver esp_http_server esp_timer console esp_netif esp_wifi)
