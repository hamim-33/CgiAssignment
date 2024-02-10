# Bresenham's Line Drawing Algorithm
### Outputs for Case 1: [(1, 1), (2, 1), (3, 2), (4, 2), (5, 3), (6, 3), (7, 4), (8, 4)]
### Outputs for Case 2: [(1, 1), (1, 2), (2, 3), (2, 4), (3, 5), (3, 6), (4, 7), (4, 8)]

## Explanation

In Bresenham's line drawing algorithm for the case of (0<m<1), changes in the x co-ordinates is larger than the y co-ordinates. So in this case we iterate over x values for finding the corresponding y values. And here the decision parameter is D = 2*dy - dx. 

But in case of m>1, changes in the y co-ordinates is larger than the x co-ordinates. So in this case the role is interchanged that means we iterate over y values for finding the corresponding x values. Therefore the decision parameter here is also changed and it is D = 2*dx - dy.

By making these adjustments, the algorithm becomes capable of handling cases where the slope m of the line is greater than 1.