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


idecore_dependencies = [core_dep]

idecore_lib = library('IdeCore', sources: sources,
                      dependencies: idecore_dependencies)


idecore_dep = declare_dependency(link_with: idecore_lib,
                                 include_directories: uppsrc_inc)
