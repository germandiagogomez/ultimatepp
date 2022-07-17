sources = ['IconDraw.cpp',
           'AlphaCtrl.cpp',
           'RGBACtrl.cpp',
           'ImageOp.cpp',
           'Paint.cpp',
           'Event.cpp',
           'Fast.cpp',
           'IconDes.cpp',
           'List.cpp',
           'Image.cpp',
           'Smoothen.cpp',
           'Text.cpp',
           'Bar.cpp',
           'EditPos.cpp',
           'ImlFile.cpp']

gtk_dep = dependency('gtk+-3.0')

icondes_lib = library('IconDes', sources: sources,
                   include_directories:
                     [uppsrc_inc],
                   dependencies: gtk_dep)

icondes_dep = declare_dependency(link_with: icondes_lib,
                                 include_directories: uppsrc_inc,
                                dependencies: gtk_dep)
