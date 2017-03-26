# libmpv

libmpv headers and linking libraries

Linking libraries are only provided for `win32`, and `win32-x64` will be added. For other operating systems, use `pkg-config` and system-wide libmpv


## Windows - how to generate `mpv.lib`

This `mpv.lib` for Windows was generated using the instructions on [MPV's wiki](https://github.com/mpv-player/mpv/blob/master/DOCS/compile-windows.md#linking-libmpv-with-msvc-programs) from the [srsfckn MPV windows builds](https://mpv.srsfckn.biz) Dev package. 


### x86

```
CALL "C:\Program Files (x86)\Microsoft Visual Studio 14.0\VC\vcvarsall.bat" x86
lib /def:mpv.def /name:mpv-1.dll /out:mpv.lib /MACHINE:X86
```

### x64

```
CALL "C:\Program Files (x86)\Microsoft Visual Studio 14.0\VC\vcvarsall.bat" x64
lib /def:mpv.def /name:mpv-1.dll /out:mpv.lib /MACHINE:X64
```

