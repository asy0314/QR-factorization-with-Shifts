# QR-Factorization-with-Shifts
Almost upper triangular; Givens; Single-Shift vs. Wilkson shifts; Breaking symmetry

The main file is Driver.jl. Please run Driver.jl

# contents of function_code.jl
a: reduce a symmetric matrix A to Hessenberg form using Householder reflections
operate in place, overwriting the input matrix with Hessenberg form

b: run a single iteration of the unshifted QR algorithm 
using Givens rotations to implement QR factorization on T_k
input = T_k hessenberg from 
output = T_{k+1} Hessenberg form

c: ren the practical QR iteration with both the Single-Shift and Wilkinson Shift. 
using QR iteration in b, with criteria for when to implement deflation and when to terminate QR iteration    

d: design an experiment that evaluates your practical QR algorithm with shifts
include a semi-log plot showing the rate of convergence of Single-Shift and Wilkinson Shift to compare
