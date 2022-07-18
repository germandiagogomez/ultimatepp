sources = ['SystemDraw.cpp',
           'Frame.cpp',
           'CtrlMt.cpp',
           'Ctrl.cpp',
           'CtrlChild.cpp',
           'CtrlPos.cpp',
           'CtrlDraw.cpp',
           'CtrlMouse.cpp',
           'CtrlKbd.cpp',
           'CtrlTimer.cpp',
           'CtrlClip.cpp',
           'LocalLoop.cpp',
           'Preedit.cpp',
           'CtrlCoreInit.cpp',
           'TopWindow.cpp',
           'DrawWin32.cpp',
           'DrawOpWin32.cpp',
           'DrawTextWin32.cpp',
           'ImageWin32.cpp',
           'MetaFile.cpp',
           'UtilWin32.cpp',
           'Win32Ctrl.cpp',
           'Win32Wnd.cpp',
           'Win32Clip.cpp',
           'Win32DnD.cpp',
           'Win32Proc.cpp',
           'TopWin32.cpp',
           'DHCtrl.cpp',
           'DrawX11.cpp',
           'DrawOpX11.cpp',
           'DrawTextX11.cpp',
           'ImageX11.cpp',
           'UtilX11.cpp',
           'X11Ctrl.cpp',
           'X11Wnd.cpp',
           'X11Proc.cpp',
           'X11Clip.cpp',
           'X11DnD.cpp',
           'X11Top.cpp',
           'X11ImgClip.cpp',
           'X11App.cpp',
           'X11DHCtrl.cpp',
           'GtkDrawOp.cpp',
           'GtkDrawText.cpp',
           'GtkDrawImage.cpp',
           'GdkImage.cpp',
           'GtkUtil.cpp',
           'GtkX11Util.cpp',
           'GtkCtrl.cpp',
           'GtkCapture.cpp',
           'GtkWnd.cpp',
           'GtkCreate.cpp',
           'GtkEvent.cpp',
           'GtkTop.cpp',
           'GtkClip.cpp',
           'GtkDnD.cpp',
           'GtkApp.cpp',
           'CocoCtrl.cpp',
           'CocoWnd.cpp',
           'CocoTop.cpp',
           'CocoChSysInit.cpp',
           'ParseRTF.cpp',
           'EncodeRTF.cpp']

if host_machine.system() == 'darwin'
  add_languages('objcpp')
  sources += ['CocoDraw.mm',
            'CocoImage.mm',
            'CocoDrawText.mm',
            'CocoWin.mm',
            'CocoClip.mm',
            'CocoDrawOp.mm',
            'CocoProc.mm',
            'CocoApp.mm'
             ]
endif





gtk_dep = dependency('gtk+-3.0')

apple_frameworks = []
if host_machine.system() == 'darwin'
  apple_frameworks = dependency('appleframeworks', modules : ['AppKit',
                                                              'Foundation',
                                                              'CoreData'])
endif

ctrlcore_lib = library('CtrlCore',
                       sources: sources,
                       include_directories:
                          [uppsrc_inc],
                       implicit_include_directories: false,
                       dependencies: [gtk_dep, apple_frameworks])

ctrlcore_dep = declare_dependency(link_with: ctrlcore_lib,
                                  include_directories: uppsrc_inc,
                                  dependencies: gtk_dep)
