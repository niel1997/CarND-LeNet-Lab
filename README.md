# CarND-LeNet-Lab

## **Data**

- The data sets used in this project are contained in "traffic-signs-data". And contains the following attributes:

**Feature**

- Input picture is 28 * 28 * 1
- Training set samples: 55000
- Number of validation set samples: 5000
- Number of test set samples: 10000

**Target variable**

- Class 10

## **Implement LeNet-5**

**Architecture**

- Layer 1:Convolution Layer

Input: The original image pixel matrix (length, width, color), the size is 32 * 32 * 1.

Convolution layer parameters: The filter size is 5 * 5, the depth is 6, the padding is not all 0s, and the step size is 1.

Output: The size is 28 * 28 * 6.

Activation:Your choice of activation function.

Pooling layer

Input: The size is 28 * 28 * 6.

Pooling layer parameters: The filter size is 2 * 2, and the step length is 2 for both length and width.

Output: the size is 14 * 14 * 6.

- Layer 2:Convolution layer

Input: The size is 14 * 14 * 6.

Convolution layer parameters: The filter size is 5 * 5, the depth is 16, the padding is not all 0s, and the step size is 1.

Output: The size is 10 * 10 * 16.

Activation:Your choice of activation function.

Pooling layer

Input: The size is 10 * 10 * 16.

Pooling layer parameters: The filter size is 2 * 2, and the step length is 2 for both length and width.

Output: The size is 5 * 5 * 16.

Flatten:Flatten the output shape of the final pooling layer such that it's 1D instead of 3D.

- Layer 3:Fully connected layer

Number of input nodes: 5 * 5 * 16 = 400.

Number of parameters: 5 * 5 * 16 * 120 + 120 = 48120.

Number of output nodes: 120.

- Layer 4: Fully connected layer

Number of input nodes: 120.

Number of parameters: 120 * 84 + 84 = 10164.

Number of output nodes: 84.

- Layer 5: Fully connected layer

Number of input nodes: 84.

Number of parameters: 84 * 10 + 10 = 850.

Number of output nodes: 10.

## **Train the Model**
- The requirements and objectives of the given model training.
- Evaluate how well the loss and accuracy of the model for a given dataset.
- Train the model for a total of 10 times, and give the accuracy of each model under the verification set.

## **Evaluate the Model**
- On the test set, the model was used to predict the result, and the final accuracy was 0.988. The model effect was very good.

## **Conclusion**
- Through this study, I have a general understanding of convolutional neural network. Compared with SVM algorithm, CNN algorithm greatly reduces the computation and improves the accuracy. In this case, the accuracy of the CNN algorithm can reach 98.8% after only 10 training sessions. This not only reflects the advantages of CNN algorithm, but also has more advantages of image recognition processing, greatly expanding the application range of CNN algorithm.
