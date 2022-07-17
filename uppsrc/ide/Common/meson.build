sources = ['ComDlg.cpp',
           'Module.cpp',
           'Util.cpp']

idecommon_dependencies = [core_dep, ctrllib_dep]

idecommon_lib = library('IdeCommon', sources: sources,
                        include_directories: uppsrc_inc,
                        dependencies: idecommon_dependencies)

idecommon_dep = declare_dependency(link_with: idecommon_lib,
                                  include_directories: uppsrc_inc)
