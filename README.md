# DustFFT

This is my old single-file double-precision SSE2 FFT. 
You can copy the header part into a separate file, or you
can include the C-file with `DUSTFFT_HEADER_ONLY` defined.

This version is unchanged from the 2014 version,
except for the additional real/half-complex wrappers.

While it does power-of-two only, it should be reasonably fast
and works perfectly fine at least up to a few million points.
