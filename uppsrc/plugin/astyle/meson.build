sources = [
  'ASStringTools.cpp',
  'ASBeautifier.cpp',
  'ASEnhancer.cpp',
  'ASFormatter.cpp',
  'ASResource.cpp'
]


astyle_plugin_dependencies = [
  ctrlcore_dep
]

astyle_plugin_lib = library('Astyle', sources: sources,
                            dependencies: astyle_plugin_dependencies)

astyle_plugin_dep = declare_dependency(link_with: astyle_plugin_lib)
