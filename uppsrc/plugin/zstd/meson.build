sources = [
   'Compress.cpp',
   'Decompress.cpp',
   'Util.cpp',
]


zstdupp_plugin_dependencies = [
   dependency('libzstd'),
   core_dep
]

zstdupp_plugin_lib = library('zstdupp', sources: sources,
                          dependencies: zstdupp_plugin_dependencies)

zstdupp_plugin_dep = declare_dependency(link_with: zstdupp_plugin_lib)
