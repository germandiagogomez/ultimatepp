sources = ['pngupp.cpp']

pngupp_plugin_dependencies = [
  draw_dep,
  dependency('libpng')
]

pngupp_plugin_lib = library('pngupp', sources: sources,
                            dependencies: pngupp_plugin_dependencies,
                            implicit_include_directories: false)

pngupp_plugin_dep = declare_dependency(link_with: pngupp_plugin_lib)
