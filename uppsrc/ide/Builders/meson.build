sources = [
  'CppBuilder.cpp',
  'MakeFile.cpp',
  'CCJ.cpp',
  'GccBuilder.cpp',
  'MscBuilder.cpp',
  'JavaBuilder.cpp',
  'ScriptBuilder.cpp',
  'Cocoa.cpp',
  'AndroidProject.cpp',
  'AndroidApplicationMakeFile.cpp',
  'AndroidMakeFile.cpp',
  'AndroidModuleMakeFile.cpp',
  'AndroidBuilder.cpp',
  'AndroidBuilderCommands.cpp',
  'AndroidBuilderUtils.cpp',
  'AndroidModuleMakeFileBuilder.cpp',
  'Blitz.cpp',
  'Build.cpp',
  'Install.cpp',
  'BuilderUtils.cpp']



idebuilders_dependencies = [core_dep]

idebuilders_lib = library('IdeBuilders', sources: sources,
                           include_directories:
                             [uppsrc_inc],
                           dependencies: idebuilders_dependencies)

idebuilders_dep = declare_dependency(link_with: idebuilders_lib,
                                     include_directories: uppsrc_inc)
