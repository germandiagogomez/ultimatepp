sources = ['TextDiff.cpp',
           'TextCtrl.cpp',
           'DiffCtrl.cpp',
           'DirDiff.cpp',
           'patch.cpp',
           'PatchDiff.cpp']


textdiffctrl_lib = library('TextDiffCtrl', sources: sources,
                          include_directories: [uppsrc_inc],
                          dependencies: ctrlcore_dep)

textdiffctrl_dep = declare_dependency(link_with: textdiffctrl_lib,
                  include_directories: uppsrc_inc)
