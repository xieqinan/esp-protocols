idf_build_get_property(target IDF_TARGET)

idf_component_register(SRCS "esp_mqtt_cxx.cpp"
                    INCLUDE_DIRS "include"
                    REQUIRES mqtt
                    )

target_compile_options(${COMPONENT_LIB} PRIVATE "-Wno-format")
