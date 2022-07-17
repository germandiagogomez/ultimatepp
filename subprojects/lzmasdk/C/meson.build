sources = [
  'Sha256.c',
  'Lzma2DecMt.c',
  '7zCrc.c',
  'LzmaDec.c',
  'Delta.c',
  'Lzma86Enc.c',
  'LzFind.c',
  'Threads.c',
  'LzmaEnc.c',
  'Bra.c',
  'Alloc.c',
  '7zAlloc.c',
  '7zBuf.c',
  'Ppmd7Dec.c',
  'Sort.c',
  'LzmaLib.c',
  'Xz.c',
  '7zDec.c',
  'Bcj2.c',
  'MtDec.c',
  'XzDec.c',
  'Aes.c',
  'Bra86.c',
  'XzCrc64.c',
  '7zCrcOpt.c',
  '7zStream.c',
  'Bcj2Enc.c',
  'Lzma86Dec.c',
  'XzIn.c',
  '7zArcIn.c',
  'AesOpt.c',
  '7zBuf2.c',
  '7zFile.c',
  'DllSecur.c',
  'XzEnc.c',
  'Sha256Opt.c',
  'CpuArch.c',
  'MtCoder.c',
  'BraIA64.c',
  'LzFindMt.c',
  'Ppmd7.c',
  'LzFindOpt.c',
  'XzCrc64Opt.c',
  'Lzma2Enc.c',
  'Lzma2Dec.c',
  'Ppmd7Enc.c']

add_project_link_arguments('-pthread', language: 'c')


lzma_lib = library('lzma', sources: sources)
threads_dep = dependency('threads')


lzma_dep = declare_dependency(link_with: lzma_lib,
                              include_directories: include_directories('.'),
                             dependencies: threads_dep)

meson.override_dependency('liblzmasdk',
                          lzma_dep)
