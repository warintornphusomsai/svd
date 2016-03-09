# Introduction #

Jacobi-based SVD algorithm in CUDA

# Details #
Singular Value Decomposition (SVD) is wildly used as an important tool for reducing rank. At present, the fastest method dealing with SVD of matrix has the complexity of O(m\*n\*n), which affects the speed of SVD and the scale could be dealt with. In this paper, by using the powerful capacity of floating point operation in GPU, I implemented one-sided Jacobi based SVD in CUDA, which could deal with Large-scale and dense matrix. When dealing with the matrix larger than 4096\*4096, the program in this paper is 60 times faster than the program in Matlab, and 7 times faster than MKL, which is distributed by Inter Company. The program in CUDA has improved the speed and scale of the problems dealing with SVD.