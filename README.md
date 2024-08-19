# 108TRIGO

**108TRIGO** is a Python program that applies fundamental trigonometric and hyperbolic functions to matrices. The program leverages power series expansions to compute functions like exponential, cosine, sine, and their hyperbolic counterparts on matrices provided as input.

## Overview

This project involves applying complex mathematical functions to matrices using the power series expansion method. The program is capable of calculating the exponential, cosine, sine, hyperbolic cosine, and hyperbolic sine of a matrix. It accepts matrices as command-line arguments, computes the desired function, and outputs the resulting matrix.

## Features

- **Matrix Operations**: Perform operations like exponentiation, cosine, sine, hyperbolic cosine, and hyperbolic sine on square matrices.
- **Power Series Expansion**: Uses power series to approximate these functions efficiently.
- **Error Handling**: Outputs error messages to stderr and exits with code 84 in case of issues.

## Usage

The program is designed to be run from the command line, with the following general usage:

To run the program:
```sh
python 108trigo fun a0 a1 a2 ...
```
Replace fun with the function you want to apply (EXP, COS, etc.) and provide the matrix coefficients.

## Parameters

`fun`: The function to be applied to the matrix. Supported functions are:

    `EXP` for exponential
    `COS` for cosine
    `SIN` for sine
    `COSH` for hyperbolic cosine
    `SINH` for hyperbolic sine

`a0 a1 a2 ...`: Coefficients of the matrix, provided line by line.

## Exemple

Cosine of a Matrix
```sh
python 108trigo COS 4 5 9 3 3 5 0 1 9
```
Output
```sh
0.70 -0.43 -1.94
-0.16 0.67 -1.23
-0.06 -0.15 0.07
```
Exponential of a Matrix
```sh
python 108trigo EXP 1 2 3 4
```
```diff
51.97 74.74
112.10 164.07
```
Hyperbolic Sine of a Matrix
```sh
python 108trigo SINH 1 0 2 0
```
```diff
1.18 0.00
2.35 0.00
```
