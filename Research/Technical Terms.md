## CNN
**Convolutional Neural Network** is a Technology used by AI to identify different elements in a image efficiently .It uses filters to perform convolution (**Convolution is a mathematical operation which is used to get a new function  by multiplying 2 other function values at each point where they overlap, and adding up the products***)

It breaks down the image by performing 4 operations .

*(i)Convolutional Layer* :Extracts features from the image by performing Convolutions.

*(ii)Activation layer* : This step Basically removes negative numbers thus introduces Non-linearity .

*(iii)Pooling layer* :used to reduce computational load by using Max value (Down sampling)

*(iv)Fully Connected* : Flattening the multi-dimensional map into a 1-D Vector, obtain final weights here . Softmax function is used to generate a probability of the input data.

A mutable "weight" is placed across input data which is dot product-ed with the input data , and each weight specializes in identifying a specific feature in the data like a vertical like or intensity . this Weight is what enables the AI to identify patterns in the image  

## MAC
**Multiply-and-Accumulate** ,like the name suggests , is the process of Multiplying 2 numbers and adding them to a Variable . This is one of the primary functions any AI do and This process is done millions of times . 

## Training AI
following various processes to find **Weights** 

## Inference 
Using the Trained AI to Analise new data , and the Wights are already known.

## Time Domain Signal Processing 
Data is stored as Width of a time pulse , Instead of continuous signal(Analog signal) or 1's and 0's (Digital signal). This approach generally reduce the number of hardware elements needed to compute compared to other methods of data processing . but its typically slower . 

## Kernel 
In the context of AI , its the matrix of Weight that is used on a Input data ( performing MAC) to extract features from the data .

## PE(Processing Element)
Highly specialized hardware used to do one specific function , like for exam just do MAC operations. 