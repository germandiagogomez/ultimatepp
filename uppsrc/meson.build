conf_data = configuration_data()
configure_file(input : 'uppconfig.h.in',
               output : 'uppconfig.h',
               configuration : conf_data)


uppsrc_inc = include_directories('.')

add_project_arguments(
  ['-DflagGUI',
  '-DflagGCC',
  '-DflagSHARED',
  '-DflagPOSIX',
  '-DflagLINUX',
  '-DflagMAIN'],
  language: 'cpp')



# Libraries
subdir('CppBase')
subdir('Core')
subdir('CtrlCore')
subdir('Draw')

# Plugins
subdir('plugin')


# Continue with libraries
subdir('HexView')
subdir('CtrlLib')
subdir('Esc')
subdir('RichText')
subdir('CodeEditor')
subdir('Painter')
subdir('RichEdit')

subdir('PdfDraw')
subdir('IconDes')
subdir('Report')
subdir('TabBar')
subdir('TextDiffCtrl')


# TheIde
subdir('ide')

