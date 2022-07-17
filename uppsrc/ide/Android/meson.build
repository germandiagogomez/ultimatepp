sources = [ 'Android.cpp',
            'AndroidSDK.cpp',
            'AndroidNDK.cpp',
            'Apk.cpp',
            'AndroidManifest.cpp',
            'Adb.cpp',
            'LogCat.cpp',
            'NDKBuild.cpp']


ideandroid_dependencies = [core_dep, pcre_plugin_dep]


ideandroid_lib = library('IdeAndroid', sources: sources,
                         include_directories:
                           [uppsrc_inc],
                         dependencies: ideandroid_dependencies)

ideandroid_dep = declare_dependency(link_with: ideandroid_lib,
                                    include_directories: uppsrc_inc)
