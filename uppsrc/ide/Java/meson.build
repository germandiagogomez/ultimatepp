sources = [
  'JavaVersion.cpp',
  'Java.cpp',
  'Jdk.cpp']


idejava_lib = library('IdeJava', sources: sources,
                      include_directories:
                        [uppsrc_inc])

idejava_dep = declare_dependency(link_with: idejava_lib,
                  include_directories: uppsrc_inc)
