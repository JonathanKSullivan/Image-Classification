# Deep Learning Foundations Nanodegree 
## Neural Networks
### Project: My First Neural Network
## Overview

In this project, I classified images from the CIFAR-10 dataset. The dataset consists of airplanes, dogs, cats, and other objects. The dataset was to be preprocessed, then trained on a convolutional neural network. I normalized the images, one-hot encoded the labels, build a convolutional layer, max pool layer, and fully connected layer. At the end, you can see its predictions on the sample images.

![My First Neural Network](./images/main.jpg)

## Getting Started

### Environment
#### Running floydhub.com

1. Create an account on [floydhub.com](https://www.floydhub.com) (don't forget to confirm your email). You will automatically receive 100 free GPU hours. 

2. Install the `floyd` command on your computer:

        pip install -U floyd-cli
        
    Do this even if you already installed `floyd-cli` before, just to make sure you have the most recent version (Its pace of development is fast!).

3. Associate the command with your Floyd account:

        floyd login

    (a page with authentication token will open; you will need to copy the token into your terminal)


4. Enter the folder for the image classification project:

        cd image-classification

5. Initiate a Floyd project:

        floyd init dlnd_image_classification

6. Run the project:

        floyd run --gpu --env tensorflow --mode jupyter --data diSgciLH4WA7HpcHNasP9j

    It will be run on a machine with GPU (`--gpu`), using a Tenserflow environment (`--env tensorflow`), as a Jupyter notebook (`--mode jupyter`), with Floyd's built-in cifar-10 dataset  available (`--data diSgciLH4WA7HpcHNasP9j`).
    
7. Wait for the Jupyter notebook to become available and then access the URL displayed in the terminal (described as "path to jupyter notebook"). You will see the notebook.

8. Remember to explicitly stop the experiment when you are not using the notebook. As long as it runs (even in the background) it will cost GPU hours. You can stop an experiment in the ["Experiments" section on floyd.com](https://www.floydhub.com/experiments) or using the `floyd stop` command:

        floyd stop ID
 
    (where ID is the "RUN ID" displayed in the terminal when you run the project; if you lost it you can also find it in the ["Experiments" section on floyd.com](https://www.floydhub.com/experiments))

## Built With
## Authors
* **Udacity** - *Initial work* - [Deep Learning Repo](https://github.com/udacity/deep-learning)
* **Jonathan Sulivan**

## Acknowledgments
* Hackbright Academy
* Udacity


<a rel="license" href="http://creativecommons.org/licenses/by-nc-nd/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-nd/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc-nd/4.0/">Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License</a>. Please refer to [Udacity Terms of Service](https://www.udacity.com/legal) for further information.


