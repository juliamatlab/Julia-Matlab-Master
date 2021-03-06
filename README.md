<p align="center">
  <img src="https://github.com/juliamatlab/Julia-Matlab-Master/blob/master/logo/Julia-Matlab-Logo.png" alt="Julia-Matlab-Logo" height="400"/>
</p>


 [![Dev Doc](https://img.shields.io/badge/docs-dev-blue.svg)](https://juliamatlab.github.io/MatLang/dev)

# Julia-Matlab-Master
Master repository for JuliaMatlab organization which provides Matlab friendly API for functions and packages in Julia language.

## Goal
The purpose of this organization is to make Julia more like a home for Matlab users.

## Structure
For each Matlab toolbox a Julia native package is created, that provides several Julia functions that mimic Matlab's functionality in that toolbox.

### List of packages (toolboxes)
* **[MatLang](https://github.com/juliamatlab/MatLang)**: API for Matlab's language core functions  [![Dev Doc](https://img.shields.io/badge/docs-dev-blue.svg)](https://juliamatlab.github.io/MatLang/dev)

### List of Functions in Each package
The list of the functions that are implemented can be found here:

<table>
    <tr>
        <td></td>
        <td>package (toolbox)</td>
        <td></td>
    </tr>
    <tr>
        <td>1</td>
        <td>MatLang</td>
        <td>clcM</td>
        <td>zerosM, onesM, randM, eyeM, trueM, falseM, diagM, catM, horzcatM, vertcatM, repelemM(limited), repmatM, linspaceM, logspaceM, meshgridM, ndgridM, freqspaceM, lengthM, sizeM, numelM, isscalarM, isvectorM, sortM, flipM, fliplrM, flipudM, flipdimM, rot90M, transposeM, squeezeM</td>
        <td>doubleM, singleM, int8M, int16M, int32M, int64M, uint8M, uint16M, uint32M, uint64M</td>
    </tr>
</table>


The full list of the functions that will be implemented in the future can be found [here](https://www.mathworks.com/help/matlab/referencelist.html;jsessionid=e221a09e47ed26d2b333ea600f68?type=function)


## Developing / Coding Standard
For coding standard please refer to [Coding Standard](https://github.com/juliamatlab/Julia-Matlab-Master/blob/master/Coding-Standard.md).
Feel free to contribute to this multi-field project. We need developers from different backgrounds to provide Matlab friendly API and wrappers.

Separate repositories are created for each toolbox. To provide fast and efficient wrappers please follow: https://docs.julialang.org/en/v1/manual/performance-tips/#Write-%22type-stable%22-functions-1

## Benchmark (Julia vs Matlab)
Here in [Julia-Matlab-Benchmark](https://github.com/juliamatlab/Julia-Matlab-Benchmark) repository you can see the benchmarks for the functions that are implemented in this organization. A function that is implemented is tested both in Julia and Matlab to compare the speed.

<p align="middle">
  <img src="https://raw.githubusercontent.com/juliamatlab/Julia-Matlab-Benchmark/master/Figures/Matlab_Julia-1-BLAS-Thread_Julia-MKL/Figure16.png" alt="K-means Run Time" width="400"/>
  <img src="https://raw.githubusercontent.com/juliamatlab/Julia-Matlab-Benchmark/master/Figures/Matlab_Julia-1-BLAS-Thread_Julia-MKL/Figure4.png" alt="Matrix Quadratic Form" width="400"/>
</p>


## Background
**Matlab** is a commercial language that has many users especially in Academia. **Julia** is an open-source scientific programming language that was designed from the beginning for high performance, i.e. it is a high-level fast language!


## Reference
The idea of this repository was inspired by [Julia_for_MATLAB_Users](https://en.wikibooks.org/wiki/Julia_for_MATLAB_Users/Index) and [MatlabCompat](https://github.com/MatlabCompat/MatlabCompat.jl), and [GNU Octave](https://www.gnu.org/software/octave/)


## Disclaimer

All the codes that are presented in this organization are written in the open source Julia language from scratch and by no means or intentions present a complete overlap with product of Mathworks Inc., nor any intentions to violate any of materials copyrighted by Mathworks Inc. or any other respective third party copyright owner. The codes are written using native Julia packages and published state-of-the-art algorithms, being property of the public domain. Any overlap with property of respective copyright owners is pure accidental.
