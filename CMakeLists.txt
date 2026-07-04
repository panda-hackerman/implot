add_library(implot STATIC
        implot.h
        implot_internal.h
        implot.cpp
        implot_items.cpp
        implot_demo.cpp
)

target_include_directories(implot PUBLIC .)
target_link_libraries(implot PUBLIC imgui)

set_target_properties(implot PROPERTIES
        CXX_STANDARD 11
        CXX_STANDARD_REQUIRED ON)