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

|   n |   qsort-fixed-pivot |   qsort-random-pivot |
|-----|---------------------|----------------------|
|  10 |               0.075 |                0.086 |
| 100 |               4.164 |                0.464 |
| 200 |               4.553 |                0.877 |
| 300 |               9.590 |                1.308 |
| 400 |              17.621 |                1.994 |
| 500 |              26.731 |                2.461 |
| 600 |              40.732 |                2.808 |
| 700 |              52.291 |                3.470 |
| 800 |              75.920 |                4.029 |
| 900 |              89.697 |                6.902 |



Random Order: 

|   n |   qsort-fixed-pivot |   qsort-random-pivot |
|-----|---------------------|----------------------|
|  10 |               0.037 |                0.039 |
| 100 |               0.351 |                0.399 |
| 200 |               0.717 |                0.991 |
| 300 |               1.089 |                1.839 |
| 400 |               1.510 |                2.086 |
| 500 |               2.144 |                2.645 |
| 600 |               5.430 |                6.175 |
| 700 |               2.887 |                4.050 |
| 800 |               3.119 |                3.963 |
| 900 |               4.298 |                5.096 |




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


