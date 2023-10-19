This is a college project that utilizes successive over-relaxation to solve an N-dimensional linear system. It uses a python notebook and ensures an efficient solution through sparse matrices.

# Problem statement
The approximate solution T of Laplace's equation ∇2 T = 0 in a 
two-dimensional domain Discretized square using a uniform grid (xi = x0 + ih ; yj = y0 + jh) 
can be obtained solving the system of linear equations that arises from applying 
the following operator to each one of the grid nodes

4Ti j − Ti−1 j − Ti+1 j − Ti j−1 − Ti j+1 = 0

The behavior of the SOR method is analyzed, and a then we determine the distribution of heat over a region of a computer's motherboard.

![image](https://github.com/Maferep/SOR-TemperatureSimulator/assets/62344533/3f5f5ff5-b217-42ba-8ad4-08507ad69406)


The figure shows the discretization of a square domain whose sides were divided into N = 4 equal parts, 
which will give an approximate solution T in the (N-1) x (N-1) interior nodes of the grid, 
while in the boundaries the value of T is imposed (TN, TS, TW, TE on each of the edges). 
Numbering the nodes as shown in Figure approximate solution T in the interior nodes 
is obtained as a solution of a linear equations whose matrix of coefficients and independent term,
for N = 4, acquires the following structure:

![image](https://github.com/Maferep/SOR-TemperatureSimulator/assets/62344533/b299df53-d723-4056-b257-af096ff9d2aa)

## Tasks
a) Apply the operator indicated in (1) to the problem posed and determine the structure to be used. acquires matrix A for a generic N value. Analyze whether the structure acquired by the matrix It depends on how you number the nodes. 

b) Write a program to apply the SOR method to the problem posed, considering how data the values of N, RTOL and w. 

c) Apply the developed program considering RTOL = 0.01, N = 4 and variable w (1.00, 1.05, 1.10,..., 1.95). 

d) Repeat considering N = 32. Keep in mind to only operate with non-null elements of A to be able to solve this case without excessive memory requirements.

e) Present the results obtained by plotting the number of iterations needed to converge in each case as a function of w. In the same graph present the following estimate empirical ρ(TSOR) ≈ R1/n where R is the tolerance achieved and n is the number of iterations carried out on a case-by-case basis. 

f) Verify whether the data obtained experimentally correspond to the theoretical values of ρ(TGS), woptimum, and ρ(TSOR). Write conclusions.

### Part 2
The system discussed in Part 1 applies to a region of the motherboard of a computer where memories are going to be placed. 
Therefore, we want to know the temperature distribution in that area.
Temperatures in the study area can be calculated by solving the equation of Laplace taking the boundary conditions 
TN, TS, TW, TE of the last 4 digits of the number multiplied by 10. For example, for ID 123456, 
TN = 30, TS = 40, TW = 50, TE = 60. 
Each group must report the temperature value in the center corresponding to their data.
It also asks to plot the isolines (or isobands) of the temperature calculated in the form of two-dimensional or, 
failing that, graph the temperature distribution according to slices horizontal or vertical using Cartesian diagrams. 
Take N = 8, RTOL = 0.001 and w = woptimal to perform these calculations.

# Warnings

Some translations to English are pending.
