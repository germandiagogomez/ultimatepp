sources = ['Lay.cpp',
'Iml.cpp',
'Sch.cpp',
'Util.cpp',
'Base.cpp',
'Item.cpp',
'ItemDisplay.cpp',
'CodeBrowser.cpp',
'TopicBase.cpp',
'Reference.cpp',
'File.cpp',
'Topic.cpp',
'Template.cpp',
'Link.cpp',
'TopicWin.cpp',
'Move.cpp',
'CodeRef.cpp',
'TopicI.cpp']


idebrowser_dependencies = [dependency('gtk+-3.0')]

idebrowser_lib = library('IdeBrowser', sources: sources,
                         include_directories:
                           uppsrc_inc,
                         dependencies: idebrowser_dependencies)


idebrowser_dep = declare_dependency(link_with: idebrowser_lib)
