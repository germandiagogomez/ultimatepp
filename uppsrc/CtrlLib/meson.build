
sources = [
  'LabelBase.cpp',
  'DisplayPopup.cpp',
  'Button.cpp',
  'Switch.cpp',
  'EditField.cpp',
  'Text.cpp',
  'LineEdit.cpp',
  'DocEdit.cpp',
  'ScrollBar.cpp',
  'HeaderCtrl.cpp',
  'ArrayCtrl.cpp',
  'MultiButton.cpp',
  'PopupTable.cpp',
  'DropList.cpp',
  'DropChoice.cpp',
  'Static.cpp',
  'Splitter.cpp',
  'FrameSplitter.cpp',
  'SliderCtrl.cpp',
  'ColumnList.cpp',
  'Progress.cpp',
  'AKeys.cpp',
  'RichTextView.cpp',
  'Prompt.cpp',
  'Help.cpp',
  'DateTimeCtrl.cpp',
  'SuggestCtrl.cpp',
  'Bar.cpp',
  'MenuItem.cpp',
  'MenuBar.cpp',
  'ToolButton.cpp',
  'ToolBar.cpp',
  'ToolTip.cpp',
  'StatusBar.cpp',
  'TabCtrl.cpp',
  'TreeCtrl.cpp',
  'DropTree.cpp',
  'DlgColor.cpp',
  'ColorPopup.cpp',
  'ColorPusher.cpp',
  'FileList.cpp',
  'FileSel.cpp',
  'FileSelUtil.cpp',
  'PrinterJob.cpp',
  'Windows.cpp',
  'Win32.cpp',
  'Gtk.cpp',
  'TrayIconWin32.cpp',
  'TrayIconX11.cpp',
  'TrayIconGtk.cpp',
  'Update.cpp',
  'CtrlUtil.cpp',
  'CtrlLibInit.cpp',
  'LNGCtrl.cpp',
  'Ch.cpp',
  'ChWin32.cpp',
  'ChGtk3.cpp',
  'ChCoco.cpp'
]

ctrllib_dependencies = [ctrlcore_dep, dependency('libnotify')]

if host_machine.system() == 'darwin'
  add_languages('objcpp')
  sources += ['Cocoa.mm',
              'ChCocoMM.mm',
              'MacMenu.mm']
  ctrllib_dependencies += [dependency('appleframeworks', modules: 'cocoa')]
endif




ctrllib_lib = library('CtrlLib',
                      sources: sources,
                      implicit_include_directories: false,
                      include_directories:
                      [uppsrc_inc],
                      dependencies: ctrllib_dependencies)

ctrllib_dep = declare_dependency(link_with: ctrllib_lib,
                                 include_directories: uppsrc_inc,
                                 dependencies: ctrlcore_dep)
