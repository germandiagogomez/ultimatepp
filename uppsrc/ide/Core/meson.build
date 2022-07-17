sources = ['Ide.cpp',
           'Core.cpp',
           'Builder.cpp',
           'Hdepend.cpp',
           'Assembly.cpp',
           'Package.cpp',
           'Workspace.cpp',
           'usc.cpp',
           'BinObj.cpp',
           'Logger.cpp',
           'Util.cpp',
           'Host.cpp']



idecore_lib = library('IdeCore', sources: sources,
                      include_directories:
                        [uppsrc_inc])

idecore_dep = declare_dependency(link_with: idecore_lib,
                                 include_directories: uppsrc_inc)
