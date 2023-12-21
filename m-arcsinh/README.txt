import tensorflow as tf
from sklearn.neural_network import MLPClassifier
import numpy as np
from sklearn import svm
from sklearn import datasets
from sklearn.model_selection import train_test_split
from sklearn.metrics import accuracy_score
from sklearn.metrics import precision_score
from sklearn.metrics import recall_score
from sklearn.metrics import f1_score

import time





Notable packages that are needed are tensorflow, sklearn, time, and numpy. The attached .ipynb file outputs the results that are noted in our study and goes through each of the 5 datasets we are testing. 
It also details how to replicate the gamma results noted in the study. Tensorflow and numpy are used to define the m-arcsinh activation function for MLP, Time is used to get training time performance, sklearn is needed for metric scores, datasets, and their SVM implementation.