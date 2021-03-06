# Online-Generation-of-Low-Discrepancy-Sequence

This repository contains the code and results reported in the paper Online generation of low-discrepancy sequences: from Monte-Carlo to Quasi-Monte-Carlo by retrying

Given an infinite sequence of i.i.d. uniform random variables on $[0,1)^d$, we construct an efficient online algorithm to select a subsequence that achieves a discrepancy of $O(d \log_2^{2d+1} N / N)$ simultaneously for all $N \in \mathbb{N}$, with respect to the class of axis-aligned hyper-rectangles.
The algorithm uses the power of one retry, a recent variant of the celebrated  power of two choices, and is guaranteed to discard an arbitrarily small portion of the samples and never more than one out of two consecutive samples.
In order to make its decision of whether to discard the $N$-th uniform or not, it needs $O(dN \log_2^{d-1} N)$ space, and uses $O(d\log_2^d N)$ time. Our discrete-time algorithm is analyzed via the concentration of carefully constructed continuous-time point processes that maintain balance over hierarchies of Haar wavelet functions.
In addition, we describe a simpler greedy-retry' strategy, that we conjecture achieves a near-optimal discrepancy of $O(d\log_2^{d+1} N)$. Finally, we provide an efficient implementation and detailed simulations in one and two dimensions, that support our main theorem and conjecture.
