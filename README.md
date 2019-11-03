# Thought-Experiments
This repository will contain my thought experiments conducted in the field of Deep Learning. 

1. [Meow_and_Woof](https://github.com/ayulockin/Thought-Experiments/blob/master/Meow_and_Woof.ipynb): Uses 1D colvolution for audio classification of Cat and Dog. Achieved 83% train and 75% val on basic architecture. Nothing fancy. 

    I had this thing in my head going for sometime that 1D Conv like 2D conv can capture simplified feature in the initial layers. Like for an image classification the initial layer usually end up being an edge detector. So I thought the initial layer for 1D conv or audio classification will be some envelope like psd or hilbert or homomorphic. 

    And it turned out that it's true.

    [Nbviewer](https://nbviewer.jupyter.org/github/ayulockin/Thought-Experiments/blob/master/Meow_and_Woof.ipynb)

2. [DirectionCNN_with_MNIST](https://github.com/ayulockin/Thought-Experiments/blob/master/DirectionCNN_with_MNIST.ipynb): A simple MNIST handwritten digit classifier. The idea behind this notebook is to see what will happen if the input image is flipped upside down. The flipping operation which changed the shape of the digit entirely is "new data" to the model. And hence false prediction. 

    I think that even though initial layers extract simple features. The features are highly dependent on the type of image it has seen. A simple experiment like this showed that CNN, rather Neural Network in itself does not capture the `sense of direction`. This theory can be proved on images such as chess pieces, which do not change the overall appearance of the image. We humans too can classify a fliped 5 as 2. But certainly, a king(chess piece) will be king even if we flip the image. 
    
    Is there a method that can capture this sense of direction? Obviously, if we label and consider this problem in a supervised setting it can be achieved. How do humans get that the image is flipped and most of the times we recognize the image? 
    
    I do understand that we can easily overcome this issue by training the model with such examples. Can I call this experiment a very poor demonstration of adversarial learning(attack)?
    
3. Coming soon. 
    
    
