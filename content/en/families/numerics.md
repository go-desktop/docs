---
title: "CPU, SIMD & numerics"
weight: 120
---

# CPU, SIMD & numerics {#cpu-simd-numerics}

Getting the machine's width out of pure Go, on all six 64-bit targets — and the scientific stack built on top of it, measured against NumPy, SciPy and mpmath rather than against itself.

| Organisation | Repos | Site | Docs | What it holds |
| --- | --- | --- | --- | --- |
| [`go-asmgen`](https://github.com/go-asmgen) | 1 | [site](https://go-asmgen.github.io/) | [docs](https://go-asmgen.github.io/docs/) | Ergonomic generation of Go-compatible Plan 9 assembly for every 64-bit Go target. |
| [`go-simd`](https://github.com/go-simd) | 23 | [site](https://go-simd.github.io/) | [docs](https://go-simd.github.io/docs/) | SIMD kernels on all six of Go's 64-bit targets — codecs, hashes, string scans, bitsets, float and int8 dot products. |
| [`go-ndarray`](https://github.com/go-ndarray) | 1 | [site](https://go-ndarray.github.io/) | [docs](https://go-ndarray.github.io/docs/) | A numpy-shaped n-dimensional array, with GEMM at vecLib parity. |
| [`go-fft`](https://github.com/go-fft) | 1 | [site](https://go-fft.github.io/) | [docs](https://go-fft.github.io/docs/) | Fast Fourier transforms at numpy and scipy accuracy, without FFTW. |
| [`go-numerics`](https://github.com/go-numerics) | 3 | [site](https://go-numerics.github.io/) | [docs](https://go-numerics.github.io/docs/) | The three pieces a numerical program reaches for after the array: special functions (gamma, beta, erf, Bessel, zeta), optimisation and root finding, and quadrature with ODE solvers including the stiff ones (Radau, BDF). |
| [`go-statistics`](https://github.com/go-statistics) | 1 | [site](https://go-statistics.github.io/) | [docs](https://go-statistics.github.io/docs/) | Probability distributions, descriptive statistics and hypothesis tests, with accuracy measured against mpmath rather than against another Go implementation. |
| [`go-approx`](https://github.com/go-approx) | 2 | [site](https://go-approx.github.io/) | — | Interpolation, splines and smoothing, and polynomials in the Chebyshev, Legendre, Hermite and Laguerre bases — validated against SciPy and NumPy. |
| [`go-sparse`](https://github.com/go-sparse) | 1 | [site](https://go-sparse.github.io/) | [docs](https://go-sparse.github.io/docs/) | Sparse matrices, the orderings that make them tractable (RCM, AMD, COLAMD), and iterative solvers. |
| [`go-dsp`](https://github.com/go-dsp) | 1 | [site](https://go-dsp.github.io/) | [docs](https://go-dsp.github.io/docs/) | Signal processing: filter design and filtering, spectral estimation, resampling and peak finding, following SciPy and MATLAB. |
| [`go-bignum`](https://github.com/go-bignum) | 1 | [site](https://go-bignum.github.io/) | [docs](https://go-bignum.github.io/docs/) | Correctly rounded elementary functions and constants on math/big.Float, at any precision and in every rounding mode — what the accuracy of everything above is checked against. |
| [`go-dataframe`](https://github.com/go-dataframe) | 1 | [site](https://go-dataframe.github.io/) | [docs](https://go-dataframe.github.io/docs/) | Labelled columnar tables: DataFrame and Series, CSV, Parquet and Arrow, group-by, joins and time series. |
| [`go-plot`](https://github.com/go-plot) | 1 | [site](https://go-plot.github.io/) | [docs](https://go-plot.github.io/docs/) | Matplotlib-class figures for the stack above, to SVG, PNG and the screen, with real LaTeX in labels. |
| [`go-notebook`](https://github.com/go-notebook) | 2 | [site](https://go-notebook.github.io/) | [docs](https://go-notebook.github.io/docs/) | Notebooks over that stack: a reactive compiled kernel that keeps its values and orders cells by what they use, and a browser playground that interprets the cells in WebAssembly while the libraries they call stay compiled. |
| [`go-scikit`](https://github.com/go-scikit) | 2 | [site](https://go-scikit.github.io/) | — | The parity programme for the stack as a whole — an inventory, a bibliography and a measured status against MATLAB and Mathematica — plus its Ruby bindings. |

Counts are public repositories that hold code; brand, docs and landing
repositories are excluded.
