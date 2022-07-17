sources = ['TabBar.cpp',
           'FileTabs.cpp',
           'TabBarCtrl.cpp']


tabbar_lib = library('TabBar', sources: sources,
                   include_directories:
                     [uppsrc_inc],
                    dependencies: ctrllib_dep)

tabbar_dep = declare_dependency(link_with: tabbar_lib)
