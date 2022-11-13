# Beauty-Classification
Successfully established a deep learning model which can precisely classify female facial images into mainly two classes, beautiful and average.

![Beauty Classification](https://etrain.xyz/assets/img/posts/SCUT-FBP5500-score.png)
![Beauty Classification](https://miro.medium.com/max/1068/1*NoAGOF-PE6_QoLoqCeMesg.png)

## Context

This data set was created to determine if a CNN could be trained to classify female facial images into one of two classes, Beautiful or Average. I have always had a preoccupation with faces. In particular I was curious as to how we seem to have a built in pattern recognition system in our brains that differentiates people by their facial morphology. This differentiation can take many forms but one of the most common is our seemingly subconscious classification of beauty. So I decided if a CNN could be trained to make a similar classification. Towards this end I gathered 2000 images of fashion models from all over the world to use as the images for the Beautiful data set. I then gathered 2000 images selected from the CELEB data set. From that data set I selected women that appeared to be in about the same age range as the fashion models but that I thought were of "average" appearance. Of course this is MY interpretation of average which will differ from what others might consider as average. Thus there is a natural bias in the selection. I used a similar process to select the images for the Validation set and the test set. I also included in the data set a Consolidated data set which combines the training, test and validation images into a single data set. This is useful for those that wish to create their own training, test and validation splits.

## Content

The data set consists of a training set, a test set, a validation set and a consolidated set. Each of these sets contains two folders labeled as Beautiful and Average. For the training set there are 2000 images in the Beautiful folder and 2000 images in the Average folder. For the test set there are 150 images in the beautiful folder and 150 images in the Average folder. The validation set is similarly divided into 150 images of each type. The consolidated folder 2300 images in the Beautiful folder and 2300 images in the Average folder. The consolidated folder combines the images from the training, test and validation sets into a single set. This is convenient for users that want to create their own splits of training, test and validation images.
All images are 224 X 224 X 3 color jpg images. Images have been cropped to only show the face. All data sets were run through a duplicate image detector and all duplicate images were removed to prevent leakage between the data sets.

## Acknowledgements

Images for the "Average" female images were selected from the CELEB data set.

## Inspiration

The CNN I used demonstrates very high accuracy on the classification of the test set. I am concerned however that since I selected what I considered to be "Average" female faces that the results are heavily biased my MY opinion. I would be eager to know what the results would be if the user selects faces to feed into the trained model for classification and see if they agree with the classification.
