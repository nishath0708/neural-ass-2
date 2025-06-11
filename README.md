# neural-ass-2
https://drive.google.com/file/d/1gqz3CDOGPIeYaePiJ-X2_MdlEyTGZ6Qb/view?usp=sharing
https://github.com/nishath0708/neural-ass-2/edit/main/README.md
NISHANTH SAI KURUGUNTLA
700766566
Question 1: Convolution Operations with Different Parameters

Step 1: Define the Input Matrix
A 5x5 input matrix is reshaped to (1, 5, 5, 1) to match the Conv2D input format.

Step 2: Define the Kernel
A 3x3 Laplacian-style kernel is used for edge detection and reshaped to (3, 3, 1, 1).

Step 3: Apply Convolution
A function is created to perform convolution with different stride and padding values. The Conv2D layer is initialized and the weights (kernel) are manually set.

Step 4: Results
Convolution is tested with:

Stride = 1, Padding = 'valid'
Stride = 1, Padding = 'same'
Stride = 2, Padding = 'valid'
Stride = 2, Padding = 'same'
Each output is printed to observe changes in output size and pattern.

Question 2: CNN Feature Extraction with Filters and Pooling

Task 1: Edge Detection using Sobel Filter

Step 1: Load Grayscale Image
The image is loaded using OpenCV in grayscale mode.

Step 2: Apply Sobel Filter
Sobel filters are applied in X and Y directions to detect vertical and horizontal edges.

Step 3: Display Results
The original, Sobel-X, and Sobel-Y images are displayed using matplotlib.

Task 2: Max Pooling and Average Pooling
Step 1: Create Random Input
A random 4x4 matrix is created and reshaped to (1, 4, 4, 1) for CNN input.

Step 2: Apply Pooling

Max Pooling: captures strong features
Average Pooling: averages values and smooths
Step 3: Display Output
Prints the original, max pooled, and average pooled matrices for comparison.

Question 3: Data Preprocessing – Standardization vs. Normalization

Step 1: Load Dataset
The Iris dataset is loaded using load_iris() from sklearn.datasets.

Step 2: Apply Scaling

Min-Max Normalization: scales features to [0, 1]
Z-score Standardization: scales features to mean = 0, std = 1
Step 3: Model Training
A Logistic Regression model is trained and tested on:

Original data
Min-Max Normalized data
Z-score Standardized data
Step 4: Distribution Visualization
Histograms are plotted for each feature in original, normalized, and standardized forms.

task 5
Explanation – Normalization vs. Standardization

Use Normalization when features need to be in a fixed range (e.g., [0,1]), common in neural networks using sigmoid or tanh.
Use Standardization when data has outliers or varies widely, better for models with ReLU or batch normalization.
Summary

This assignment demonstrates:

How stride and padding affect CNN outputs
How Sobel filters extract directional edges
The role of pooling in dimensionality reduction
The effect of preprocessing methods on model performance
Visual inspection of feature scaling techniques
Use the following command to launch TensorBoard: tensorboard --logdir logs/fit/
