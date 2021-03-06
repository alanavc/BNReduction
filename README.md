Requirements:
1. Install Macaulay2 (http://www.math.uiuc.edu/Macaulay2/)
2. Download Boost Library 1.55.0 (http://www.boost.org/doc/libs/)
NOTE: If you want to use a different version of the Boost Library, you will have to edit the file NetReductionBoost/Makefile accordingly (Step 3 in Compiling)
3. Download BNReduction.zip
4. Have gcc, g++, perl, bash

Compiling:
1. Unzip BNReduction.zip
2. Move the Boost Library folder to the BNReduction folder
3. Make sure the contents of the file NetReductionBoost/Makefile and your version of the Boost Library match (only necessary if using a different version of Boost Library).
4. Go to BNReduction
5. make clean
6. make install
7. ./Testing_BNReduction.sh (this is used to check that everything is working)

Usage:  
./BNReduction.sh inputfile
The file with steady states will be generated into inputfile.fp (if it has no lines, that means there are no fixed points)
NOTE: The input file must be a file where each line has a Boolean function for each variable. E.g., the following is a Boolean network in 4 variables:
x1 & x2
0
!x2 | x4
1
The variables must range from x1 to xn. The folder Examples has some examples of Boolean networks in the necessary format.

How to cite: 
1. A. Veliz-Cuba, B. Aguilar, F. Hinkelmann and R. Laubenbacher. Steady state analysis of Boolean molecular network models via model reduction and computational algebra. BMC Bioinformatics, 2014.

Additional references:
2. A. Veliz-Cuba, B. Aguilar, and R. Laubenbacher. Dimension Reduction of Large Sparse AND-NOT Network Models. Electronic Notes in Theoretical Computer Science. Accepted, 2014. (see also arxiv.org/abs/1311.6868).
3. A. Veliz-Cuba, K. Buschur, R. Hamershock, A. Kniss, E. Wolff and R. Laubenbacher. AND-NOT logic framework for steady state analysis of Boolean network models. Applied Mathematics and Information Sciences. 7(4): 1263-1274, 2013.
4. A. Veliz-Cuba. Reduction of Boolean Network Models. Journal of Theoretical Biology, 289:167-172, 2011.
5. F. Hinkelmann, M. Brandon, B. Guang, R. McNeill, G. Blekherman, A. Veliz-Cuba and R. Laubenbacher. ADAM: Analysis of Discrete Models of Biological Systems Using Computer Algebra. BMC Bioinformatics, 12:295, 2011.
6. A. Veliz-Cuba, A. Jarrah and R. Laubenbacher. The Polynomial Algebra of Discrete Models in Systems Biology. Bioinformatics, 26:1637-1643, 2010.
References 2-6 cover all the mathematical theory behind reference 1.

License: Free for any academic/educational/any other non-profit use; in which case, you can do whatever you want with this code. No restrictions of any kind, explicit or implied. 

For commercial purposes it is still free for up to a month (for evaluation). Afterwards, please contact the authors.

Warranty: No warranty of any kind, explicit or implied. 

