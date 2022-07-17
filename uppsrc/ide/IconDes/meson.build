sources = [
  'IconDes.cpp',
  'IdeDes.cpp']


ideicondes_lib = library('IdeIconDes', sources: sources,
                              include_directories:
                                [uppsrc_inc],
                              dependencies: icondes_dep)

ideicondes_dep = declare_dependency(link_with: ideicondes_lib,
                                   dependencies: icondes_dep)
