# Description

This little project explores the following assumption:
>The higher the quality of an image is, the higher is the certainty of a CNN's right classification (probability of the true label), because *better* images lead to *easier* classification and therefore more certainty. This could be proven by trying to find a correlation of the number of epochs a diffusion model was trained and the probability of the true label (the label, on which the diffusion model was trained on).

This work explores, if a CNN trained on the mnist dataset can be used to examine the quality of a diffusion model, that has been trained on the mnist model as well.
This diffusion model is only trained on mnist data that has the label "2", so that only 2s are produced by the model.

The conclusion is drawn at the end of the [main.py](main.ipynb) file. Parts of this, like the definition of the 
diffusion model, have been directly taken from the PyML course at TU Berlin or other sources (those parts are marked as 
such).