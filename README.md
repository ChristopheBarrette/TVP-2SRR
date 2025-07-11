This folder contains the necessary files to replicate the analysis presented in Goulet Coulombe (2025) and generate Figure 3 from his study. It includes the dataset, example code, and essential functions.

Contents :
- Dataset: Canadian data used for the analysis.
- Example Code: The MATLAB code utilized to generate Figure 3 in Goulet Coulombe (2025).
- Functions/Tools: A suite of MATLAB functions for analysis.

Files and Functions
1.	tvp_2SRR:
- Description: Estimates the residuals and companion matrix of a reduced-form VAR using Ridge regression and the two-step Ridge regression method proposed in Goulet Coulombe (2025).
- Usage: Call this function to perform the main analysis as described in the paper.
3.	IRF_tvp_2SRR:
- Description: Computes the impulse response functions (IRFs) for a given reduced-form VAR model. IRFs show how shocks to one variable propagate through the system over time.
- Usage: Use this function to visualize the impact of shocks on the variables over specified periods.
4.	CVmultivariate2:
-	Description: Performs cross-validation to determine the optimal lambda for a multivariate Ridge regression model. Lambda controls the amount of regularization applied to the model, affecting the time-variation in the regression coefficients.
-	Usage: Run this function to find the lambda value that minimizes the mean squared error (MSE) of the model.
5.	dualGRR:
-	Description: Estimates parameters of a dual Ridge regression model, including coefficients and variance components. It accommodates various settings such as co-integration and generalized cross-validation.
-	Usage: Utilize this function for estimating parameters in dual Ridge regression scenarios.
6.	Zfun:
-	Description: Generates the expanded matrix Z′ (Z prime) required for the Two-Step Ridge Regression (2SRR) procedure. This matrix includes the original data matrix X and additional columns of lagged variables.
-	Usage: Employ this function to prepare the matrix Z′ for 2SRR analysis.

7.	fXMAT:
-	Description: Prepares matrices for performing a Vector Autoregression (VAR) with a specified lag length.
-	Usage: Use this function to set up the matrices required for VAR analysis.
8.	Cumulzeros:
-	Description: Processes a binary matrix X by performing logical negation and identifying blocks of consecutive values. The transformed matrix Z replaces the end of each zero-block with the negative length of the preceding one-block and computes the matrix ZX by element-wise multiplying X with the cumulative sum of ZZ.
-	Usage: Apply this function to handle and transform binary matrices for further analysis.

Running the Example Code
1.	Set Path: Update the file path in the first section of the example code to match your local directory.
2.	Execute Code: Run the rest of the code to replicate the results and generate Figure 3.


