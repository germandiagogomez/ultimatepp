sources = ['Painter.cpp',
           'SvgArc.cpp',
           'PainterPath.cpp',
           'DrawOp.cpp',
           'Painting.cpp',
           'PaintPainting.cpp',
           'Xform2D.cpp',
           'Approximate.cpp',
           'Stroker.cpp',
           'Dasher.cpp',
           'Transformer.cpp',
           'Rasterizer.cpp',
           'RasterizerClip.cpp',
           'RenderChar.cpp',
           'Fillers.cpp',
           'Context.cpp',
           'Path.cpp',
           'Render.cpp',
           'Image.cpp',
           'Mask.cpp',
           'Gradient.cpp',
           'RadialGradient.cpp',
           'OnPath.cpp',
           'SvgUtil.cpp',
           'SvgBounds.cpp',
           'SvgStyle.cpp',
           'SvgParser.cpp']


painter_lib = library('Painter', sources: sources,
                   include_directories:
                     [uppsrc_inc])

painter_dep = declare_dependency(link_with: painter_lib,
                                include_directories: [uppsrc_inc])
