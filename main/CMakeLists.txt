file(
    GLOB_RECURSE
        SOURCES
            *.c
)

idf_component_register(
    SRCS ${SOURCES}
    INCLUDE_DIRS
        .
    REQUIRES
        console
        nvs_flash
        esp_wifi
        littlefs
        ftpserver
)