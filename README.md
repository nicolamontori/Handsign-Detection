# Handsign-Detection
Final project for the "Zero to GANs course" - Python machine learning aaplication to detect handsign from images.

## Objective
The objective of this quick project was to test the capabilities of the ADAM algo to train on image detection.
In particular, I used a dataset borrowed from ('https://github.com/ardamavi/Sign-Language-Digits-Dataset') which contains pictures of handsigns that display numbers. 
The AI had to be able to recognize the number displaied from the hand in the picture.

## Initialization
First thing first we need to install all the libraries required to run this little project: most notably pytorch and in particular torchvision.
After that, we import the dataset from the github link I provided previously. The data is already polished and organized, pretty much ready to go.
Despite that, we still want to know information on the dataset structure, so we run some code to find out the classes present and the dimension of the dataset.

## Training
After we analised the dataset structure, we split the dataset into different parts to work with it. We select a random seed, we set the dimension of the testing and training datasets.
After that we proced to define our model in the code. Once defined, we test the availability of hardware acceleration and GPU power, to speed things up for us.
We can now finally test the model and evaluate its baseline loss and accuracy.
This is the most critical part: defining the hyperparameters is the most difficult part here, because it relies for the most part on trial and error. 
After a few tries I ended up choosing the ADAM algo and the learn rate of 0.0001 on 25 epochs.

## Evaluating Results
Using the Matplot Libraries we can visualize the return of our training on very simple plots.
We can also call a few test images and try the model on a case by case situation.
The final metrics logged were:
-Loss: 0.064
-Accuracy: 0.980
These are almost optimal results, it is probably possible to improve a little bit on these, but it's probably not worth time it would take for a very marginal improvement.

## Thanks
I would like to thank freeCodeCamp.org and the Jovian.ml creators for the amazing opportunity for having such an inspiring course all online for free, with platforms available to discuss the projects.
Ad maiora semper.
