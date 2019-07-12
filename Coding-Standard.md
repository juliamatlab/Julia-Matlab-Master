# Coding Standard
In the following we discuss some Matlab's syntax and how we are going to implement it in Julia.

### Packages names
Package names will follow the following format: `MatToolboxName`. For example, for image processing toolbox, the package name will be `MatImageProcessing`.

### Functions names
In Julia, a capital `M` is added to the name of the all the functions. For example `eig` will be implemented as `eigM`.

### Functions with multiple input
In Julia, we use multiple methods for a function instead of using `varargin`.

### Dispatching multiple methods for a function
In Julia, for now, we will use `if` and `elseif`.

### Function's additional options:
In Matlab, usually options are passed to the functions by strings (e.g. `function(args,'optionName',optionValue)`. However In Julia, we use `function(args,optionName=optionValue)`. If  in Matlab syntax the `optionValue` is a string, we use `:optionValue` instead in Julia.

* Example 1 - in Matlab option is a single string:

  In Matlab, ``eig(A,B,algorithm)``, `algorithm` is a string that can have values of `'chol'` or `''qz''`.

  In Julia this will be `eig(A,B,algorithm=:chol)` or `eig(A,B,algorithm=:qz)`.

* Example 2 - in Matlab option and its value are a string pair:

  In Matlab, `plot(x,y,'Color','red')`, `'Color'` and its value `'red'` are a pair of strings. 
 
  In Julia, we use `plot(x,y,Color=:red)` instead.

* Example 3 -  in Matlab option is a string and its value a number:

  In Matlab, `plot(x,y,''LineWidth',0.5)`, `'LineWidth'` is a string and its value `0.5` is a number. 
 
  In Julia, we use `plot(x,y,LineWidth=0.5)` instead.

### Matlab classes
In Julia, we use `struct` to define the properties of a class, then we define the methods in functions using multi-dispatching.
