idf_component_register(
    SRCS "esp_stmems_lsm9ds1.c" "include/driver/lsm9ds1_reg.c"
    INCLUDE_DIRS "include"
    REQUIRES "esp_stmems"
)

target_compile_options(${COMPONENT_LIB} PRIVATE "-Wno-format" "-Wno-maybe-uninitialized" "-Wno-incompatible-pointer-types")
