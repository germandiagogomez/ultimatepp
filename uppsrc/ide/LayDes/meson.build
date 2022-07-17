sources = [
  'sdiff.cpp',
  'laylib.cpp',
  'layusc.cpp',
  'property.cpp',
  'textprop.cpp',
  'fontprop.cpp',
  'propane.cpp',
  'item.cpp',
  'layout.cpp',
  'visgen.cpp',
  'laydes.cpp',
  'layfile.cpp',
  'laywin.cpp']



idelaydes_lib = library('IdeLayDes', sources: sources,
                              include_directories:
                                ['.',
                                 uppsrc_inc],
                                dependencies: ctrllib_dep)

idelaydes_dep = declare_dependency(link_with: idelaydes_lib)
