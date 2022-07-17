sources = [
  'Png.cpp',
  'Img.cpp',
  'Qtf.cpp',
  'HexView.cpp',
  'TreeDes.cpp',
  'Xml.cpp',
  'Json.cpp',
  'md.cpp',
]

idedesigners_dependencies = [core_dep, ctrlcore_dep]

idedesigners_lib = library('IdeDesigners', sources: sources,
                         include_directories:
                           [uppsrc_inc],
                         dependencies: idedesigners_dependencies)

idedesigners_dep = declare_dependency(link_with: idedesigners_lib,
                                     dependencies: ctrlcore_dep)
