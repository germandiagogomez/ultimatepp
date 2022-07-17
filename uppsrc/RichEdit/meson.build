sources = ['UnitEdit.cpp',
           'Editor.cpp',
           'Speller.cpp',
           'Kbd.cpp',
           'Mouse.cpp',
           'Cursor.cpp',
           'Undo.cpp',
           'Modify.cpp',
           'Formating.cpp',
           'FormatDlg.cpp',
           'ParaFormat.cpp',
           'TableUndo.cpp',
           'Table.cpp',
           'Find.cpp',
           'Tool.cpp',
           'Clip.cpp',
           'StyleKeys.cpp',
           'Ruler.cpp',
           'HeaderFooter.cpp']

gtk_dep = dependency('gtk+-3.0')

richedit_lib = library('RichEdit', sources: sources,
                       include_directories:
                          [uppsrc_inc],
                       dependencies: gtk_dep)

richedit_dep = declare_dependency(link_with: richedit_lib,
                                 include_directories: uppsrc_inc)
