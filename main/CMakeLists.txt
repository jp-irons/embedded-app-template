file(GLOB_RECURSE APP_EMBED_FILES "app_files/files/*")

idf_component_register(
    SRCS
        app_main.cpp
        ApplicationContext.cpp
        LoggingConfig.cpp
        app/TemperatureHandler.cpp
        app_files/AppFileTable.cpp
    REQUIRES
        auth
        device
        esp_platform
        network_store
        framework
        framework_files
        http
    