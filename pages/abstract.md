---
title: Abstract
permalink: /abstract/
---

# Abstract

This article introduces HODLR3D, a class of hierarchical matrices arising out of $N$ body problems in three dimensions. HODLR3D relies on the fact that certain off-diagonal matrix subblocks arising out of the $N$ body problems in three dimensions are numerically low-rank. For the Laplace kernel in $3$D, which is widely encountered, we prove that all the off-diagonal matrix subblocks are rank deficient in finite precision. We also obtain the growth of the rank as a function of the size of these matrix subblocks. For other kernels in three dimensions, we numerically illustrate a similar scaling in rank for the different off-diagonal subblocks. We leverage this hierarchical low-rank structure to construct HODLR3D representation, with which we accelerate matrix-vector products. The storage and computational complexity of the HODLR3D matrix-vector product scales almost linearly with system size. We demonstrate the computational performance of HODLR3D representation through various numerical experiments. Further, we explore the performance of the HODLR3D representation on distributed memory systems.

 HODLR3D developed in the article can be viewed as an extension to HODLR and [HODLR2D](https://arxiv.org/abs/2204.05536) in three dimensions.
