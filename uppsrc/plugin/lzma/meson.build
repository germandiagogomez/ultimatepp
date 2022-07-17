sources = ['lzma.cpp']

lzmaupp_plugin_dependencies = [
  core_dep,
  dependency('zlib'),
  dependency('liblzma'),
  dependency('liblzmasdk')
]

lzmaupp_plugin_lib = library('lzmaupp', sources: sources,
                             dependencies: lzmaupp_plugin_dependencies)


lzmaupp_plugin_dep = declare_dependency(link_with: lzmaupp_plugin_lib)
