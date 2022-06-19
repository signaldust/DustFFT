# DustFFT

This is my old single-file double-precision SSE2 FFT. 
You can copy the header part into a separate file, or you
can include the C-file with `DUSTFFT_HEADER_ONLY` defined.

While it compiles as C++ the performance is known to be better
at least with some compilers when compiled as regular C.

It also has a scalar version as a fall-back for unaligned,
but if you want compile it on non-x86 platforms, then you'll
have to edit the SSE versions out (or include something like
[sse2neon](https://github.com/DLTcollab/sse2neon)).

This version is unchanged from the 2014 version, except for the
additional real/half-complex wrappers.

While it does power-of-two only, it should be reasonably fast
and works perfectly fine at least up to a few million points
and has been written to be somewhat cache-aware.
