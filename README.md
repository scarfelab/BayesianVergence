# BayesianVergence
### The code accompanies the paper “A Bayesian model of distance perception from ocular convergence” by Peter Scarfe and Paul Hibbard.

The code runs in Mathematica/Wolfram:
https://www.wolfram.com

The code can also be accessed via the free Wolfram Player:
https://www.wolfram.com/player/

Or free Wolfram Engine:
https://www.wolfram.com/engine/

Part of the code also needs the Mathstatica toolbox (however, an alternative derivation is provided which avoids the use of this toolbox):
http://www.mathstatica.com

The files (Wolfram Notebooks) are as follows:

**BayesianVergence2025**: is the code which derives the model and plots Figures 4, 5, 6 and 7 in the paper. The code has a toggle to save out figures and two equations (posterior probability distributions).

**makeResposeDistributions**: loads in the equations produced by BayesianVergence2025 and calculates response distributions and saves these out to file. It also produces Figure 8 and 9 in the paper. To avoid the use of the Mathstatica plugin we provide these files dircetly (distancePDFa and vergencePDFa).

**responseDistributionSurface**: loads in the data produced by makeResposeDistributions and plots Figure 9 in the paper. 

**flatVergencePrior**: derives the distance prior which would be consistent with a flat vergence prior. 

**Alternative Derivation**: provides an alternative way to derive the model which uses plain Mathematica and does not need Mathstatica.

Much of the code makes use of the parallel processing functionality of Mathematica. Running without parallel processing would be substantially slower. 
The notebooks are extensively documented. The code should be run in the following order (1) BayesianVergence2025, (2) makeResposeDistributions and (3) responseDistributionSurface. This is due to the data being saved out and loaded. 

