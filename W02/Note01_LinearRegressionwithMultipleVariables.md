##Linear Regression with Multiple Variables

####Environment Setup Instructions
####Octave Tutorial
#####Basic Operations
- = : assign
- == : equal 
- ~= : not equal
- xor(a,b)
- c = (3>=1) ----> c = 1 (check true or false)

>a = 3; % semicolon supressing output
>disp(sprintf('2 decimals: %0.2f', a)) % C program style print

- format long / format short
- Matrix: 
    A = [1 2; 3 4; 5 6]
    A = [1 2;
    3 4;
    5 6]
    
- V = [1 2 3] vs V = [1; 2; 3] vs V = 1:0.1:2

#####Moving Data Around
- Use 'length' only for Vector to avoid the confusion when use for matrix
- pwd: current directory
- cd: change directory
- ls: list of files on the directory

- load('xxx.dat')
- who: data variables in current session
- whos: more detailed info of who

- clear __variable__: delete a __variable__
- clear: delete all variables

- save xxx.mat v : save v to the file xxx.mat (mat saves as binary)
- save xxx.txt v : save v as text (ASCII)

- A .* B  *
- A .^ 2
- 1 ./ v
- 1 ./ A
- log(v)
- exp(v)
- abs(v)
- -V % -1*v       *
- v + ones(length(v),1)

- A' : transpose
- ind: index
- max : column-wise maximum
- find(a < 3): returns column number
- pinv(A): create the inverse 


#####Plotting Data
#####Control Statements
#####Vectorization
