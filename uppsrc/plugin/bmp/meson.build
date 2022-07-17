sources = ['Bmp.cpp',
           'BmpWrite.cpp',
           'Icon.cpp']

bmpupp_plugin_dependencies = [draw_dep]


bmpupp_plugin_lib = library('bmpupp', sources: sources,
                          dependencies: bmpupp_plugin_dependencies)

bmpupp_plugin_dep = declare_dependency(link_with: bmpupp_plugin_lib)
