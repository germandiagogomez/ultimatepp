sources = ['gifupp.cpp']

gifupp_plugin_dependencies = [
  dependency('giflib')
]

gifupp_plugin_lib = library('gifupp', sources: sources,
                          dependencies: gifupp_plugin_dependencies)

gifupp_plugin_dep = declare_dependency(link_with: gifupp_plugin_lib)
