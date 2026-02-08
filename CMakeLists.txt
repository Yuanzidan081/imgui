set(ImGUI_Root ${CMAKE_CURRENT_SOURCE_DIR})
set(ImGUI_Src 
    ${ImGUI_Root}/imgui.cpp
    ${ImGUI_Root}/imgui_demo.cpp
    ${ImGUI_Root}/imgui_draw.cpp
    ${ImGUI_Root}/imgui_tables.cpp
    ${ImGUI_Root}/imgui_widgets.cpp
    )   
set(ImGUI_Include 
    ${ImGUI_Root}
    ${ImGUI_Root}/backends
    )
add_library(imgui STATIC ${ImGUI_Src})

target_include_directories(imgui PUBLIC ${ImGUI_Include})
