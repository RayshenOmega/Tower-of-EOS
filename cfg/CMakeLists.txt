add_library(Config STATIC
    config.cpp
)
target_precompile_headers(Config PRIVATE pch.hpp)
target_link_libraries(Config nlohmann_json::nlohmann_json)