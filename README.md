# Self Organizing Maps based Clustering for Keystroke Dynamics
This repository contains the extraction of relevant features from the data and process of keystroke dynamics by performing a dimensionality reduction using Kohonen Self Organising Maps a.k.a SOMs and inturn, do the unsupervised classification and authentication of users

# Steps for Data Acquisition:

>def extract_keylog_features(path) 
Refer: keystroke_festure_extractor.py
This functons takes the keylog features with the timestamp in two cases ie... hold time for a particular key and transition time between 2 keys pressed. 

Note: This functions also eliminates the cases of outliers where the time stored for the key pressed is >1 sec.

The data for the different individuals is then, loaded in the Jupyter Notebook and further processing is done.

Different 

The training of an SOM is governed by hyperparameters, initial learning rate η0, learning rate decay time τη, initial neighbourhood size σ0, neighbourhood size decay rate τσ. For every epoch t of training they are updated to learning rate η and neighbourhood size σ respectively. 

Used values of Hyperparameters for the implementation:

> num_epochs = 1000
> eta_0 = 1
> sigma_0 = 8
> t_eta = 500
> t_sigma = 650
> n = 15

Libraries Used:
1. numpy
2. matplotlib
3. standard 
