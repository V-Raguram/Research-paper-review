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
## Psum 
**Partial sums** are intermediate values obtained while performing a **MAC** operation 
## Training AI
following various processes to find **Weights** 

## Inference 
Using the Trained AI to Analise new data , and the Wights are already known.

## Time Domain Signal Processing 
Data is stored as Width of a time pulse , Instead of continuous signal(Analog signal) or 1's and 0's (Digital signal). This approach generally reduce the number of hardware elements needed to compute compared to other methods of data processing . but its typically slower . 

## Kernel 
In the context of AI , its the matrix of Weight that is used on a Input data ( performing MAC) to extract features from the data .

## PE(Processing Element)
Highly specialized hardware used to do one specific function ; for example just do MAC operations. 

## Spatial Architecture 
Grid of independent PEs arranged in such a way that they can work in parallel and pass data to one other . this is mainly used to keep the data in these SA for as long as possible to avoid the data movement from memory to the PEs .( AS lot of time and energy is spent in moving Data from memory to PEs ) 

## Network-On-Chip
Interconnects provided on the chip which connects different components with each other , used primarily to transfer data .

## SPads(Scratch Pads)
Tiny local memory used to store small data for calculation , present in the PE itself. 

## Multicast 
its a Communication technique where data from point A is sent to multiple points (B,C,D,etc) at the same time in one clock cycle .

## Data gating 
A logic circuit which stops the PE from performing calculation if multiplication with 0 is deducted as this operation always leads to 0.  

## Input Feature maps (IFMAP)
Basically the input pixel (Data)

