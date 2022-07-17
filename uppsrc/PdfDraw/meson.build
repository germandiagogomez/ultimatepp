sources = ['TTFStream.cpp',
           'TTFStruct.cpp',
           'TTFSubset.cpp',
           'TTFReader.cpp',
           'PdfDraw.cpp',
           'PdfReport.cpp']


pdfdraw_lib = library('PdfDraw', sources: sources,
                      include_directories:
                        [uppsrc_inc])

pdfdraw_dep = declare_dependency(link_with: pdfdraw_lib,
                                include_directories: uppsrc_inc)
