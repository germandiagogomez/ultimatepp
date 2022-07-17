sources = [
  'MacroElement.cpp',
  'MacroManager.cpp',
  'UscFileParser.cpp']


idemacromanager_lib = library('IdeMacroManager', sources: sources,
                              include_directories:
                                [uppsrc_inc],
                              dependencies: [core_dep, ctrllib_dep])

idemacromanager_dep = declare_dependency(link_with: idemacromanager_lib,
                                         dependencies: ctrllib_dep)
