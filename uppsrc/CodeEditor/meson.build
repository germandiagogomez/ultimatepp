sources = [
  'Register.cpp',
  'HighlightOut.cpp',
  'Syntax.cpp',
  'Style.cpp',
  'RegisterSyntax.cpp',
  'CSyntax.cpp',
  'CInit.cpp',
  'CHighlight.cpp',
  'CLogic.cpp',
  'DiffSyntax.cpp',
  'TagSyntax.cpp',
  'PythonSyntax.cpp',
  'LogSyntax.cpp',
  'EditorBar.cpp',
  'FindReplace.cpp',
  'Lang.cpp',
  'CodeEditor.cpp'
]

codeeditor_dependencies = [
  ctrllib_dep,
  pcre_plugin_dep
]


codeeditor_lib = library('CodeEditor', sources: sources,
                   include_directories:
                     [uppsrc_inc],
                   dependencies: gtk_dep)

codeeditor_dep = declare_dependency(link_with: codeeditor_lib,
                  include_directories: uppsrc_inc)
