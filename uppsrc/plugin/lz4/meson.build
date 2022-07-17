sources = [
 'Compress.cpp',
 'Decompress.cpp',
 'util.cpp'
]


lz4upp_plugin_dependencies = [core_dep]


lz4upp_plugin_lib = library('lz4upp', sources: sources,
                         dependencies: lz4upp_plugin_dependencies)

lz4upp_plugin_dep = declare_dependency(link_with: lz4upp_plugin_lib)
