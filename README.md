![Julia-Matlab-Logo](https://github.com/juliamatlab/Julia-Matlab-Master/Julia-Matlab-Logo.png)

# Julia-Matlab-Master
Master repository for JuliaMatlab organization which provides Matlab friendly API for functions and packages in Julia language.

## Goal
The purpose of this organization is to make Julia more like a home for Matlab users.

## Background
**Matlab** is a commercial language that has many users especially in Academia. **Julia** is an open-source scientific programming language that was designed from the beginning for high performance, i.e. it is a high-level fast language! Because of these reasons Julia is considered an excellent replacement for Matlab.

## Structure
For each Matlab toolbox a Julia native package is created, that provides several Julia functions that mimic Matlab's functionality in that toolbox.

### List of packages (toolboxes)
* **[MatMath](url)**: API for math functions
* **[MatString](url)**: API for string function
* **[MatImage](url)**: API for image processing toolbox functions  
* **[MatVision](url)**: API for computer vision toolbox functions   

### List of Functions in Each package
The list of the functions that are implemented can be found here:

| package (toolbox)  |            |         |        |        |         |     |     |           |       |
|-------------|------------|---------|--------|--------|---------|-----|-----|-----------|-------|
| MatMath  |  |    |  |  |  |  |  |  |  |
| MatString          |        |         |        |        |         |     |     |           |       |
| MatImage   |       |      |        |        |         |     |     |           |       |
| MatVision |        |  |  |        |         |     |     |           |       |


The full list of the functions that will be implemented in the future can be found here: https://www.mathworks.com/help/matlab/referencelist.html;jsessionid=e221a09e47ed26d2b333ea600f68?type=function

## Developing
Feel free to contribute to this multi-field project. We need developers from different backgrounds to provide Matlab friendly API and wrappers.

Separate repositories are created for each toolbox. To provide fast and efficient wrappers please follow: https://docs.julialang.org/en/v1/manual/performance-tips/#Write-%22type-stable%22-functions-1

## Benchmark (Julia vs Matlab)
Here in [Julia-Matlab-Benchmark](https://github.com/juliamatlab/Julia-Matlab-Benchmark) repository you can see the benchmarks for the functions that are implemented in this organization. A function that is implemented is tested both in Julia and Matlab to compare the speed.

![K-means Run Time](https://raw.githubusercontent.com/aminya/MatlabJuliaMatrixOperationsBenchmark/master/Figures/Figure16.png
)




The idea of this repository was inspired by https://en.wikibooks.org/wiki/Julia_for_MATLAB_Users/Index and https://github.com/MatlabCompat/MatlabCompat.jl.
