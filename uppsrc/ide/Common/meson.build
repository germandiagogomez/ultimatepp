sources = ['ComDlg.cpp',
           'Module.cpp',
           'Util.cpp']

idecommon_lib = library('IdeCommon', sources: sources,
                        include_directories: uppsrc_inc,
                        dependencies: gtk_dep)

idecommon_dep = declare_dependency(link_with: idecommon_lib,
                                  include_directories: uppsrc_inc)
