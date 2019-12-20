# HierarchicalLearning

This work focuses on learning optimization problems with quadratical interactions
between variables, which go beyond the additive models of traditional linear learning.
We investigate more specically two dierent methods encountered in the literature to
deal with this problem: \hierNet" and structured-sparsity regularization, and study
their connections. We propose a primal-dual proximal algorithm based on an epi-
graphical projection to optimize a general formulation of these learning problems.
The experimental setting rst highlights the improvement of the proposed procedure
compared to state-of-the-art methods based on fast iterative shrinkage-thresholding
algorithm (i.e. FISTA) or alternating direction method of multipliers (i.e. ADMM),
and then, using the proposed 
exible optimization framework, we provide fair comparisons between the different hierarchical penalizations and their improvement over the
standard l1-norm penalization. The experiments are conducted both on synthetic and
real data, and they clearly show that the proposed primal-dual proximal algorithm
based on epigraphical projection is efficient and effective to solve and investigate the
problem of hierarchical interaction learning.

***************************************************************************
* Author: Mingyuan Jiu (1), Nelly Pustelnik (2)								  
* Institutions: 
 (1,2) Zhengzhou University, China
 (2) Univ Lyon, Ens de Lyon, Univ Claude Bernard, CNRS, Laboratoire de Physique, F-69342 Lyon, France 
* Date: Sep, 04 2019     	              									
* License CeCILL-B                                    								
***************************************************************************


*********************************************************
* RECOMMENDATIONS:                                   	*
* This toolbox is designed to work with Matlab 2009 and late version   *
*********************************************************

------------------------------------------------------------------------------------------------------------------------
#DESCRIPTION:
This toolbox provides an efficient implementation of hierarchical interaction learning with epigraphical projection for regression and multiclass SVMs.

This toolbox consists of 3 subfolder containing MATLAB functions designed for the proposed algorithm.
  ./data: the data used for demo
      ./data/reg_synthetic_data.mat: synthetic data for regression
      ./data/cls_parkinson_data.mat: classfication data constaining two classes
  ./function: the functions used in the toolbox
  ./demo: the main demo files

------------------------------------------------------------------------------------------------------------------------
#SPECIFICATIONS :

* reg_infty_epi_demo.m: It provides two algorithms for choices for regression: \ell_\infty strong hierarchy and \ell_\infty weak hierarchy;
* reg_l1_epi_demo.m: It provides two algorithms for choices for regression: \ell_1 strong hierarchy and \ell_1 weak hierarchy;
* cls_infty_epi_demo.m: It provides two algorithms for choices for multiclass SVMs: \ell_\infty strong hierarchy and \ell_\infty weak hierarchy;
* cls_l1_epi_demo.m: It provides two algorithms for choices for multiclass SVMs: \ell_1 strong hierarchy and \ell_1 weak hierarchy;

------------------------------------------------------------------------------------------------------------------------
#RELATED PUBLICATION:

M. Jiu, N. Pustelnik, S. Janaqi, M. Chebre, L. Qi and P. Ricoux
Sparse hierarchical interaction learning with epigraphical projection
accepted by Journal of Signal Processing Systems, 2019.
https://arxiv.org/abs/1705.07817

------------------------------------------------------------------------------------------------------------------------
