project (ImGUI)

set(imgui_src
    "imgui.h"
    "imgui.cpp"
    "imgui_draw.cpp"
    "imgui_widgets.cpp"
    "imgui_tables.cpp"
    "backends/imgui_impl_win32.cpp"
    "backends/imgui_impl_dx12.cpp"
)
add_library (${PROJECT_NAME} STATIC ${imgui_src})

target_include_directories (${PROJECT_NAME} PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})
