sources = ['bz2upp.cpp']

# No pkg-config in Ubuntu 18.04 for bz2
bz2_dep = dependency('bz2', required: false)
if not bz2_dep.found()
  bz2_findlib = meson.get_compiler('cpp').find_library('bz2')
  bz2_dep = declare_dependency(dependencies: bz2_findlib)
endif

bz2upp_plugin_dependencies = [
  core_dep,
  bz2_dep
]



bz2upp_plugin_lib = library('bz2upp', sources: sources,
                          dependencies: bz2upp_plugin_dependencies)

bz2upp_plugin_dep = declare_dependency(link_with: bz2upp_plugin_lib)
