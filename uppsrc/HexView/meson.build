sources = ['HexView.cpp']

hexview_dependencies = [ctrlcore_dep]

hexview_lib = library('HexView', sources: sources,
                              include_directories:
                                uppsrc_inc,
                              dependencies: hexview_dependencies)


hexview_dep = declare_dependency(link_with: hexview_lib,
                                 include_directories: uppsrc_inc)
