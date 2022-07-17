sources = ['Markdown.cpp']


mdupp_plugin_dependencies = [core_dep, dependency('md4c')]



mdupp_plugin_lib = library('mdupp', sources: sources,
                           dependencies: mdupp_plugin_dependencies)

mdupp_plugin_dep = declare_dependency(link_with: mdupp_plugin_lib)
