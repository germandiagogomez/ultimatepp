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


idedesigners_lib = library('IdeDesigners', sources: sources,
                         include_directories:
                           [uppsrc_inc],
                         dependencies: gtk_dep)

idedesigners_dep = declare_dependency(link_with: idedesigners_lib,
                                     dependencies: gtk_dep)
