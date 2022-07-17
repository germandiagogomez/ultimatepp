sources = ['jpgupp.cpp']

jpgupp_plugin_dependencies = [
  dependency('libjpeg'),
  draw_dep,
]

jpgupp_plugin_lib = library('jpgupp', sources: sources,
                            dependencies: jpgupp_plugin_dependencies)

jpgupp_plugin_dep = declare_dependency(link_with: jpgupp_plugin_lib)
