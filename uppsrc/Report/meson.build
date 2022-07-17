sources = ['Report.cpp',
           'ReportDlg.cpp']

report_lib = library('Report', sources: sources,
                     include_directories:
                       [uppsrc_inc],
                     dependencies: gtk_dep)

report_dep = declare_dependency(link_with: report_lib,
                               include_directories: uppsrc_inc)
