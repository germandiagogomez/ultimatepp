sources = [ 'RegExp.cpp']


pcre_plugin_dependencies = [dependency('libpcre'),
                            core_dep]

pcre_plugin_lib = library('Regexp', sources: sources,
                          dependencies: pcre_plugin_dependencies)

pcre_plugin_dep = declare_dependency(link_with: pcre_plugin_lib)
