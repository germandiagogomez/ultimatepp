sources = ['Font.cpp',
           'FontCR.cpp',
           'FontWin32.cpp',
           'FontFc.cpp',
           'Draw.cpp',
           'DrawText.cpp',
           'DrawData.cpp',
           'Drawing.cpp',
           'ImageAnyDraw.cpp',
           'DrawUtil.cpp',
           'DrawTextUtil.cpp',
           'Display.cpp',
           'Image.cpp',
           'ImageBlit.cpp',
           'RasterFormat.cpp',
           'RasterWrite.cpp',
           'Palette.cpp',
           'Raster.cpp',
           'RasterEncoder.cpp',
           'ImageOp.cpp',
           'ImageChOp.cpp',
           'Mify.cpp',
           'ImageScale.cpp',
           'RescaleFilter.cpp',
           'MakeCache.cpp',
           'DrawRasterData.cpp',
           'Uhd.cpp',
           'Iml.cpp',
           'DDARasterizer.cpp',
           'SDrawClip.cpp',
           'SDrawPut.cpp',
           'SDrawText.cpp',
           'SDraw.cpp',
           'SImageDraw.cpp',
           'Cham.cpp',
           'SColors.cpp']

draw_dependencies = [dependency('fontconfig')]
if host_machine.system() == 'darwin'
  add_languages('objcpp')
  sources += ['FontCoco.mm']
  draw_dependencies += [dependency('appleframeworks', modules: 'cocoa')]
endif



draw_lib = library('Draw', sources: sources,
                   include_directories:
                     [uppsrc_inc],
                  dependencies: draw_dependencies)

draw_dep = declare_dependency(link_with: draw_lib,
                  include_directories: uppsrc_inc)
