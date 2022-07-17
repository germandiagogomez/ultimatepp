sources = ['EscValue.cpp',
           'EscArray.cpp',
           'EscMap.cpp',
           'Esc.cpp',
           'EscRun.cpp',
           'EscStdLib.cpp',
           'Value.cpp']

esc_lib = library('Esc', sources: sources,
                   include_directories:
                     [uppsrc_inc])

esc_dep = declare_dependency(link_with: esc_lib,
                  include_directories: uppsrc_inc)
