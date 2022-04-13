# CMPS 2200 Reciation 6
## Answers

**Name:**_________________________


Place all written answers from `recitation-06.md` here for easier grading.

Compare running times using compare-qsort between variants of Quicksort and the provided implementation of selection sort (ssort). Perform two different comparisons: a comparison between sorting methods using random permutations of the specified sizes, and a comparison using already sorted permutations. How do the running times compare to the asymptotic bounds? How does changing the type of input list change the relative performance of these algorithms? Note that you may have to modify the list sizes based on your system memory; compare at least 10 different list sizes. The print_results function in main.py gives a table of results, but feel free to use code from Lab 1 to plot the results as well.

enter answers in answers.md

1c)

Python uses a sorting algorithm called Timsort, designed by Tim Peters. Compare the fastest of your sorting implementations to the Python sorting function sorted, conducting the tests in 3b above.

enter answers in answers.md





- **1b.**

Sorted:

|     |      n |   qsort-fixed-pivot |   qsort-random-pivot |
|-----|--------|---------------------|----------------------|
|  10 |  0.059 |               0.062 |                0.003 |
| 100 |  1.750 |               0.574 |                0.004 |
| 200 | 15.636 |               1.576 |                0.008 |
| 300 | 10.308 |               1.425 |                0.008 |
| 400 | 28.762 |               2.017 |                0.010 |
| 500 | 26.933 |               2.371 |                0.009 |
| 600 | 40.285 |               2.959 |                0.010 |
| 700 | 52.715 |               3.496 |                0.058 |
| 800 | 83.031 |               4.401 |                0.019 |
| 900 | 99.489 |               4.826 |                0.013 |



Random Order: 

|     |     n |   qsort-fixed-pivot |   qsort-random-pivot |
|-----|-------|---------------------|----------------------|
|  10 | 0.057 |               0.060 |                0.004 |
| 100 | 0.528 |               0.748 |                0.015 |
| 200 | 1.105 |               1.366 |                0.029 |
| 300 | 1.935 |               3.490 |                0.048 |
| 400 | 1.741 |               1.917 |                0.046 |
| 500 | 1.867 |               2.337 |                0.055 |
| 600 | 2.562 |               2.882 |                0.067 |
| 700 | 2.881 |               3.513 |                0.098 |
| 800 | 3.177 |               4.351 |                0.098 |
| 900 | 3.567 |               4.614 |                0.111 |




- **1c.**

Sorted:

|   n |   qsort-fixed-pivot |   qsort-random-pivot |   tim_sort |
|-----|---------------------|----------------------|------------|
|  10 |               0.087 |                0.049 |      0.003 |
| 100 |               1.291 |                0.474 |      0.004 |
| 200 |               9.001 |                2.249 |      0.008 |
| 300 |              10.227 |                1.592 |      0.007 |
| 400 |              18.561 |                1.979 |      0.008 |
| 500 |              29.431 |                2.326 |      0.009 |
| 600 |              40.288 |                2.926 |      0.010 |
| 700 |              54.617 |                3.464 |      0.010 |
| 800 |              79.534 |                4.356 |      0.013 |
| 900 |              97.409 |                4.767 |      0.011 |




Random Order:


|   n |   qsort-fixed-pivot |   qsort-random-pivot |   tim_sort |
|-----|---------------------|----------------------|------------|
|  10 |               0.060 |                0.074 |      0.004 |
| 100 |               0.600 |                2.497 |      0.015 |
| 200 |               1.191 |                1.036 |      0.024 |
| 300 |               1.119 |                1.383 |      0.036 |
| 400 |               1.514 |                1.939 |      0.041 |
| 500 |               1.943 |                2.396 |      0.052 |
| 600 |               2.224 |                2.877 |      0.066 |
| 700 |               2.855 |                3.386 |      0.079 |
| 800 |               3.232 |                4.518 |      0.120 |
| 900 |               3.792 |                4.640 |      0.102 |


