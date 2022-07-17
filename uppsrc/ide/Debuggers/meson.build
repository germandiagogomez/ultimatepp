sources = [
  'Disas.cpp',
  'GdbCmd.cpp',
  'GdbData.cpp',
  'Gdb.cpp',
  'GdbMem.cpp',
  'GdbUtils.cpp',
  'Cpu.cpp',
  'Debug.cpp',
  'Mem.cpp',
  'Sym.cpp',
  'Exp.cpp',
  'PrettyUpp.cpp',
  'PrettyStd.cpp',
  'Pretty.cpp',
  'Visualise.cpp',
  'Terminal.cpp',
  'Data.cpp',
  'Tree.cpp',
  'Stack.cpp',
  'Code.cpp',
  'Pdb.cpp']


idedebuggers_dependencies = [core_dep, ctrlcore_dep]

idedebuggers_lib = library('IdeDebuggers', sources: sources,
                      include_directories:
                         [uppsrc_inc],
                      dependencies: idedebuggers_dependencies)


idedebuggers_dep = declare_dependency(link_with: idedebuggers_lib,
                                     dependencies: ctrlcore_dep)
