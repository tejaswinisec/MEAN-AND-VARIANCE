# MEAN-AND-VARIANCE-USING-SCILAB
AIM: To write a program for mean, variance and cross correlation in SCILAB and verify the output.

EQUIPMENTS Needed

· Computer with i3 Processor · SCI LAB

Algorithm

Define the Function: Specify the function you want to simulate. For example, f(x)=sin⁡(x)f(x) = \sin(x)f(x)=sin(x) or any other function.

Generate Sample Points: Decide on the range and the number of sample points. Generate these sample points within the desired range.

Evaluate the Function: Compute the function values at each of these sample points.

Compute Mean, Variance and Cross Correlation: Use Scilab's functions to calculate the mean and variance of the computed function values.

Display Results: Output the computed mean variance and Cross Correlation

PROCEDURE

· Refer Algorithms and write code for the experiment.

· Open SCILAB in System

· Type your code in New Editor

· Save the file

· Execute the code

· If any Error, correct it in code and execute again

· Verify the generated results

PROGRAM
```asm
clear;
clc;
clear;
function z = f(x)
    z = 3*(1 - x)^2
endfunction
a = 0;
b = 1;
EX = intg(a, b, f)
function z = c(y)
    z = 3*(1 - y)^2
endfunction
EY = intg(a, b, c)
function z = g(x)
    z = (x^2)*3*(1 - x)^2
endfunction
EX2 = intg(a, b, g)
function z = h(y)
    z = (y^2)*3*(1 - y)^2
endfunction
EY2 = intg(a, b, h)
vX2 = EX2 - (EX)^2
vY2 = EY2 - (EY)^2
disp(EX, "Mean of X =")
disp(EY, "Mean of Y =")
disp(vX2, "Variance of X =")
disp(vY2, "Variance of Y =")
x = input("Type in the reference sequence = ")
y = input("Type in the second sequence = ")
n1 = max(size(y)) - 1
r = corr(x, y, n1)
plot2d3('gnn', r)
```
OUTPUT:

<img width="740" height="685" alt="Screenshot 2025-10-23 234314" src="https://github.com/user-attachments/assets/1d12151d-20c9-4874-a059-7e693a67bf28" />


Cross Correlation

Type in the reference sequence = [1 2 3 4 5 6 7 8]

Type in the second sequence = [2 4 6 8 10 11 12 13]



calculation:
![WhatsApp Image 2025-12-04 at 12 08 05_bfe86a93](https://github.com/user-attachments/assets/5d92cd20-96cd-4647-8819-d6800df826cc)

![WhatsApp Image 2025-12-04 at 12 08 18_2e3f5d73](https://github.com/user-attachments/assets/997171fa-bb2d-4cc6-a086-e0fae0172737)


RESULT:

Thus the mean , variance and cross correlation are executed in Scilab and output is verified.****
