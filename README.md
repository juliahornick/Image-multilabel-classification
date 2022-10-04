# Image-multilabel-classification

Advances in the artificial intelligence field have been shown promising. The computational development allowed for algorithms and techniques, before never even considered, to become liable for implementation.

Machine learning algorithms have been used in several fields, such as, financial, healthcare, education and many others. Here, we will talk about a specific area: the image identification through artificial intelligence.


Working with images is a tricky thing. Besides the processing costs and storage, the process itself demands some complex techniques. Through the years several attempts were made to correctly classify images using artificial intelligence.

This project was made for a subject in the Applied Computing Program at the 
University of the State of Santa Catarina, in Brazil. It aims to identify handwritten digits from the MNIST dataset, which has around 60 thousand registers in size 28x28, from 0 to 9, this dataset is available for free on the TensorFlow lib, created by Google. The algorithm used was LightGBM, an ensemble decision tree.

This model offers a low computational cost without compromising the prediction performance.

The development of the classification project started with a data analysis, to guarantee there wasn’t any problem with the dataset. After a split in the data was made, creating two new groups: train and test dataset.

The train dataset is used so the model can learn through the data, and the test dataset is used to properly evaluate how good the model is.

A cross validation technique was also applied, using k=5, which practically means that we’ll split our train dataset into five new ones, and each dataset will also be divided in 5 parts, the algorithm will, then, use four of these parts to train and the last one to test,which will allow for a better result.

A Bayesian optimization algorithm was used to optimize the hyperparameters in the LightGBM one.

The final result was an accuracy up to 98,12%.

