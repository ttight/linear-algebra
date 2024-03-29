
# Computational Linear Algebra Use Cases

In this repo, I'll be showing a few use cases built out using Linear Algebra techniques to solve real world problems in Python projects. 


## Projects

- Number recognition using clustering in Principal Component Analysis
- Jordan Form Calculation from scratch
- Linear Transformations Applied
- Image compression using Singular Value Decomposition






### Number Recognition

In this project I wanted to show an example of how PCA is used to recognize/classify images. To do this, I use a training set of many black and white 20x20 pixel images of hand drawn numbers. Then, I use PCA to map these images to a 2 dimensional plane. By doing this I then use various clustering classification methods to find clusters of points on the 2d grid that map to the same image. Then we test out the PCA & clustering algo to attempt to predict which numbers new pictures represent. In this project, I was able to obtain a ~90% accuracy rating. Below is an example of a few images mapped onto a 2d plane. 
![Screen Shot 2023-06-04 at 4 51 55 PM](https://github.com/ttight/linear_algebra/assets/78621047/3d6f36c7-a7d0-4f4c-bfcf-96c6b39d6499)


### Jordan Form Calculation

I create a function to calculate the Jordan form (P & J Matrices) for an inputted 2x2 matrix without libraries that would overly simplify this. This shows the logic of the Jordan form calculation process directly through python logic. 

### Linear Transformations on Elipses

Python function to apply linear transformations on small matrices. In the specific example the elipse used is $(x, y) | 3x^2 - 2xy + 3y^2 = 4$, where we rotate the given elipse using the function and show the effect of different inputs. As an example, we can see the following linear transformation: 

![Screen Shot 2023-06-04 at 5 34 35 PM](https://github.com/ttight/linear_algebra/assets/78621047/e3629fe1-f4f2-48b5-8d98-ed12201d0577)


Displayed for different inputs of t: 

![Screen Shot 2023-06-04 at 5 36 43 PM](https://github.com/ttight/linear_algebra/assets/78621047/75fe24c5-4220-4e1d-9779-53e48fce0532)


### Image Compression Using Singular Value Decomposition

Given an inputted image, I compute the singular value decomposition of the R, G, B pixels of that image separately. Then show a function that given a paremeter k will show only the k singular values of that image which account for some x% of the variance in the pixels which show the image. Using this, we can show a few examples of how images become compressed or hold less data using SVD. Here's an example of the function using 20% of the singular values compared to using 80% of the singular values:

![Screen Shot 2023-06-04 at 6 09 40 PM](https://github.com/ttight/linear_algebra/assets/78621047/aae24049-1e8c-4bd0-873c-cebf9b61cf63)


