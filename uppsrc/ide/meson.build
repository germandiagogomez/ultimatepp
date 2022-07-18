subdir('Core')
subdir('IconDes')
subdir('Android')
subdir('Browser')
subdir('Builders')
subdir('Common')
subdir('Debuggers')
subdir('Designers')
subdir('Java')
subdir('LayDes')
subdir('MacroManager')


sources = [
  'BaseDlg.cpp',
  'SelectPkg.cpp',
  'UppWspc.cpp',
  'NewPackageFile.cpp',
  'Organizer.cpp',
  'Template.cpp',
  'Console.cpp',
  'FindFile.cpp',
  'FindInFiles.cpp',
  'Config.cpp',
  'ide.cpp',
  'idefile.cpp',
  'EditorTabBar.cpp',
  'Bottom.cpp',
  't.cpp',
  'Cpp.cpp',
  'Assist.cpp',
  'DCopy.cpp',
  'ContextGoto.cpp',
  'GoToLine.cpp',
  'Swaps.cpp',
  'ParamInfo.cpp',
  'Navigator.cpp',
  'Annotations.cpp',
  'Virtuals.cpp',
  'Thisbacks.cpp',
  'Log.cpp',
  'Jump.cpp',
  'MainConfig.cpp',
  'Setup.cpp',
  'Custom.cpp',
  'Print.cpp',
  'Insert.cpp',
  'idetool.cpp',
  'Install.cpp',
  'Android.cpp',
  'idebar.cpp',
  'idewin.cpp',
  'main.cpp',
  'CommandLineHandler.cpp',
  'About.cpp',
  'Macro.cpp',
  'Help.cpp',
  'SlideShow.cpp',
  'OnlineSearch.cpp',
  'Errors.cpp',
  'Calc.cpp',
  'FormatCode.cpp',
  'Abbr.cpp',
  'Qtf.cpp',
  'Xml.cpp',
  'Json.cpp',
  'MacroManager.cpp',
  'SetupSVN.cpp',
  'Upgrade.cpp',
  'UppHub.cpp',
  'MethodsCtrls.cpp',
  'Methods.cpp',
  'AutoSetup.cpp',
  'InstantSetup.cpp',
  'OutputMode.cpp',
  'Build.cpp',
  'Debug.cpp',
  'Valgrind.cpp',
  'Export.cpp',
  'RepoConsole.cpp',
  'RepoSync.cpp',
  'Credentials.cpp',
  'Diff.cpp']

ide_plugin_dependencies = [
  astyle_plugin_dep,
  pngupp_plugin_dep,
  lz4upp_plugin_dep,
  lzmaupp_plugin_dep,
  zstdupp_plugin_dep,
  bz2upp_plugin_dep,
  mdupp_plugin_dep,
  bmpupp_plugin_dep
]

apple_frameworks = []

if host_machine.system() == 'darwin'
  apple_frameworks = dependency('appleframeworks', modules : ['AppKit',
                                                              'Foundation',
                                                              'CoreData'])
endif

ide_dependencies = [
  cppbase_dep,
  core_dep,
  hexview_dep,
  ctrlcore_dep,
  draw_dep,
  esc_dep,
  report_dep,
  ctrllib_dep,
  codeeditor_dep,
  painter_dep,
  pdfdraw_dep,
  tabbar_dep,
  textdiffctrl_dep,
  richtext_dep,
  richedit_dep,
  idecore_dep,
  idecommon_dep,
  idemacromanager_dep,
  ideicondes_dep,
  ideandroid_dep,
  idebuilders_dep,
  idedesigners_dep,
  idedebuggers_dep,
  idejava_dep,
  idebrowser_dep,
  idelaydes_dep,
  dependency('x11'),
  dependency('fontconfig'),
  dependency('threads'),
  dependency('liblz4'),
  dependency('zlib'),
  dependency('libxxhash')
]



ide_exe = executable('ide', sources: sources,
                     include_directories: [uppsrc_inc, root_inc],
                     implicit_include_directories: false,
                     dependencies: [ide_dependencies, ide_plugin_dependencies,
                                   apple_frameworks])
