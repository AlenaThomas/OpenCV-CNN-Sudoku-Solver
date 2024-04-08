# OpenCV-CNN-Sudoku-Solver

Solving the sudoku puzzle using Image Processing, Artificial Intelligence and the Backtracking Algorithm!

## Procedure
1. Image Processing
The image is converted to grayscale and further Adaptive Thresholding and Dilation are applied to the image to reduce noise and enhance contours. After this happens, the coordinates of the maximum area (the sudoku grid) in the image are found.

2. Warping
Using the coordinates found, we warp the image and form individual grids on the image.These individual grids will help in extracting out the smaller tiles which contain a single digit or a blank.

3. Digit Recognition
The individual grids are passed into a convolutional neural network (Christopher) which is pretrained on a custom dataset. These grids are identified and returned in the form of a list.

4. Backtracking
The predictions are fed into a script which solves the sudoku using the Backtracking algorithm and the solution is shown on an empty sudoku grid.


## Scripts

## Scope for Improvement
