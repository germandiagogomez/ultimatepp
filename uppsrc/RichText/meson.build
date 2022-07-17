sources = [
  'Object.cpp',
  'RichImage.cpp',
  'ParaData.cpp',
  'ParaType.cpp',
  'ParaPaint.cpp',
  'HeaderFooter.cpp',
  'TxtData.cpp',
  'TxtPaint.cpp',
  'TxtOp.cpp',
  'Format.cpp',
  'TableCell.cpp',
  'TableLayout.cpp',
  'TablePaint.cpp',
  'TableData.cpp',
  'TextPaint.cpp',
  'TextStyle.cpp',
  'TextData.cpp',
  'TextTable.cpp',
  'EncodeQtf.cpp',
  'ParseQtf.cpp',
  'EncodeHTML.cpp',
  'Util.cpp'
]


richtext_lib = library('RichText', sources: sources,
                   include_directories:
                     [uppsrc_inc])

richtext_dep = declare_dependency(link_with: richtext_lib,
                  include_directories: uppsrc_inc)
