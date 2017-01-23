# RcppBrent
This package is a simple example of how to use the [BRENT C++ library](https://people.sc.fsu.edu/~jburkardt/cpp_src/brent/brent.html) inside of an R package that uses Rcpp.
According to its creator John Burkart: 
> BRENT is a C++ library which contains algorithms for finding zeros or minima of a scalar function of a scalar variable, by Richard Brent.
>
> The methods do not require the use of derivatives, and do not assume that the function is differentiable.
>
> This file includes some revisions suggested and implemented by John Denker. In particular, it is now possible to pass either a plain function or a C++ functor. Also, a "brent" namespace was defined to make it easier to avoid naming conflicts. 

The BRENT library is licensed under [Lesser GPL Version 3.0](https://people.sc.fsu.edu/~jburkardt/txt/gnu_lgpl.txt).

# Why is this useful?
The R's one-dimensional minimizer `optimize` is very handy, and there are times when one may wish to have a C++ version of the same function. The function `brent::local_min` provides exactly this.

# Helpful Hints
If you want to use the BRENT library in your Rcpp-based package, you can use RcppBrent as a template. 
Note that you the file `brent_pcb.cpp` is merely a testing file which I include here for reference.
You do not need to included it in your package to use the BRENT routines.
