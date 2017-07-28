GPE source code release.

Author  : Qingbo Wu

Version : Beta1.0

The authors are with the School of Electric Engineering, University of Electronic Science and Technology of China, Chengdu 611731, China.

===========================================================================

-------------------------COPYRIGHT NOTICE----------------------------------

Copyright (c) 2017 University of Electronic Science and Technology of China
All rights reserved.

For researchers and educators who wish to use the code for non-commercial 
research and/or educational purposes, we can provide access under the following terms:

1. Researcher shall use the code only for non-commercial research and educational purposes.
2. Researcher accepts full responsibility for his or her use of the code and shall defend and indemnify University of Electronic Science and Technology of China, including their employees, Trustees, officers and agents, against any and all claims arising from Researcher's use of the code.
3. Researcher may provide research associates and colleagues with access to the code provided that they first agree to be bound by these terms and conditions.
4. University of Electronic Science and Technology of China reserves the right to terminate Researcher's access to the Database at any time.
5. If Researcher is employed by a for-profit, commercial entity, Researcher's employer shall also be bound by these terms and conditions, and Researcher hereby represents that he or she is fully authorized to enter into this agreement on behalf of such employer.

---------------------------Instructions------------------------------------

This is a MATLAB implementation of Generic Proposal Evaluator (GPE). If this code is helpful for your research, please cite the following two papers in your bibliography, i.e.,
1. Q. Wu, H. Li, F. Meng and K. N. Ngan, "Generic Proposal Evaluator: A Lazy Learning Strategy Towards Blind Proposal Quality Assessment", IEEE Transactions on Intelligent Transportation Systems, In Press, 2017.
2. Q. Wu, H. Li, K. N. Ngan and L. Xu, "Blind Proposal Quality Assessment via Deep Objectness Representation and Local Linear Regression", IEEE International Conference on Multimedia & Expo (ICME 2017), Hong Kong, Jul. 10 - 14, 2017.
   
Usage: 

1. Locate the image and proposal files in current folder './GPE_release', 
   such as, 'traffic_sign.jpg' and 'RPN_proposal'.

2. Select a preferred mode for your project, such as,
   s.mode = 0; High Accuracy (HA) mode, with polynomial kernel
   or,
   s.mode = 1; High Efficiency (HE) mode, with linear kernel

2. Run the script demo.m to obtain proposal scores, i.e.,
   pp_score = GPE(imname,ppname,s); 

Dependencies:
LIBSVM and MATCONVNET Toolboxes have been included in current package. We 
have built their mex files under Windows 7-64bit OS. More information ab-
out how to rebuild these files across different platforms please refer to
 
http://www.csie.ntu.edu.tw/~cjlin/libsvm/

http://www.vlfeat.org/matconvnet/

If you have any suggestions or corrections in the usage of this code, plea-
se feel free to contact wqb.uestc@gmail.com
