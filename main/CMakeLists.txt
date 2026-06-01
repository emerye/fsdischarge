idf_component_register(SRCS "sntp_example_main.c" "esp_littlefs_example.c"
                    INCLUDE_DIRS "." "./include/.")
littlefs_create_partition_image(storage ../flash_data FLASH_IN_PROJECT)
