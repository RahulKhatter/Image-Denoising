# Image-Denoising
The method discussed in this report makes use of convolutional neural networks and custom keras models with custom loss functions.
The dataset used is LOL dataset which consists of 500 images, 485 of which are part of the training set and 15 are part of the evaluation set. 
The architecture of the neural network implemented is shown below. It consists of 8 convolutional layers in total. The architecture is as follows.
![download](https://github.com/RahulKhatter/Image-Denoising/assets/95233038/276cb12d-ba2e-48c4-945c-fa7a896fc9eb)
The Custom loss functions are as follows:
Color constancy loss - It corrects the color deviations that occur in the enhanced image.
Exposure loss- To prevent areas from being too dark or too bright, we use the exposure control loss. This method checks how close the average brightness of a small area is to an ideal level of 0.6.
Illumination smoothness loss-To keep the brightness changes smooth between neighboring pixels, we add the illumination smoothness loss to each curve parameter map.
Spatial consistency loss-The spatial consistency loss ensures that the enhanced image looks natural by maintaining the contrast between neighboring areas in both the original and enhanced images.


