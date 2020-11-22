![Logos](https://s3.amazonaws.com/com.twilio.prod.twilio-docs/images/jupyter_python_numpy.width-808.png)

# numpy.randomPackage

## Investigating and Explanation of numpy.random package

- Explain the overall purpose of the package.

- Explain the use of the “Simple random data” and “Permutations” functions.

- Explain the use and purpose of at least five “Distributions” functions.

- Explain the use of seeds in generating pseudorandom numbers

## Overview of numpy package

 I would like to give an overview background of numpy package before I dive into the explanation of purpose of numpy.random.
 
 NumPy is the fundamental package for scientific computing in Python. It is a Python library that provides a multidimensional array object, various derived objects (such as masked arrays and matrices), and an assortment of routines for fast operations on arrays, including mathematical, logical, shape manipulation, sorting, selecting, I/O, discrete Fourier transforms, basic linear algebra, basic statistical operations, random simulation and much more.Source: [numPy](https://docs.scipy.org/doc/numpy-1.15.0/user/whatisnumpy.html)
 
 Numpy is a specialisist package that is real efficient in dealing with arrays and numbers like matirx.
It is used for resizing, compressing and analysing. Anything scientifically you do on computer turns down to all of the ideas shows in matrix operations like, trying to compress image to a smaller size, compress song to a smaller size or trying to analysed data. This shows that matrix operations is the correct and quickest way to to do it. Therefore numpy is really essential because it knows how to deal with these kinds of operations very good. Source:[Lecture note Video](https://web.microsoftstream.com/video/b191f6b2-4d80-4ede-8b2b-62a945999585)

It is also a Python Package, specialized for building and manipulating large, multidimensional arrays. NumPy has built-in functions for linear alegbra and random number generation. It's an important library because a lot of the other Python packages such as SciPy, Matplotlib depend on Numpy to function (to a reasonable extent.) Source:[Github](https://github.com/simonava5/numpy.random/blob/master/numpy.random.ipynb)

Numpy.random number is a routine produce pseudo random numbers, using combinations of a BitGenerator to create sequences and a Generator to use those sequences to sample from different statistical distributions:
Numpy.randon package is use to generate simulated data.
Source: [NumPy.Random](https://numpy.org/doc/stable/reference/random/index.html#)

# Simple random data
******

## The use and purpose of the simple random data

******

We have four functions of simple random data:

- Intergars

- Random 

- Choice

- Byte

## integers 

This demonstration show what intergar function does and to discover how the function work and I will use documentation examples to discover how the function work, also to visualised it using histogram plot.

I will investigate Return random integers from low (inclusive) to high (exclusive), or if endpoint=True, low (inclusive) to high (inclusive). Replaces RandomState.randint (with endpoint=False) and RandomState.random_integers (with endpoint=True)
Return random integers from the “discrete uniform” distribution of the specified dtype. If high is None (the default), then results are from 0 to low.

import matplotlib.pyplot as plt

import numpy as np

rng = np.random.default_rng()

x = rng.integers(2, size=10)

x

plt.hist(x)



 
