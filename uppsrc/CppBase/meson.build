sources = ['ppconfig.cpp',
           'macro.cpp',
           'util.cpp',
           'ppfile.cpp',
           'srcfiles.cpp',
           'cpp.cpp',
           'Pre.cpp',
           'cpplex.cpp',
           'Parser.cpp',
           'Body.cpp',
           'Base.cpp',
           'ScopeInfo.cpp',
           'Qualify.cpp',
           'CppItem.cpp',
           'Expression.cpp',
           'Iface.cpp']


cppbase_lib = library('CppBase', sources: sources,
                      include_directories:
                        [uppsrc_inc])

cppbase_dep = declare_dependency(link_with: cppbase_lib,
                  include_directories: uppsrc_inc)
