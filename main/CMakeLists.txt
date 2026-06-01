idf_component_register(SRCS "sntp_example_main.c" "esp_littlefs_example.c" "discharge.c"
                PRIV_REQUIRES esp_adc
		PRIV_REQUIRES esp_event
		PRIV_REQUIRES esp_timer
		PRIV_REQUIRES nvs_flash
		PRIV_REQUIRES esp_driver_gpio
		REQUIRES esp_netif
		INCLUDE_DIRS "." "./include/.")
littlefs_create_partition_image(storage ../flash_data FLASH_IN_PROJECT)
