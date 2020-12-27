# Dealing-With-Imbalance-In-Computer-Vision

### Guidelines
In image recognition, there’s usually different kinds of imbalance issues, where majority class can have one or more orders of magnitude more instances than the minority class. The situation is worsened further in multi-class classification problem, which is often found in CV task. The ratio of training instances among different classes can be drastically different. However, it can be coarsely categorized in two types of imbalance, i.e. step imbalance and linear imbalance [1].

### Project Implementation
You will take the MNIST Dataset – uploaded for you – and create digit recognition models. You will provide code that properly handles data imbalance to accurately model the handwriting digits. In particular, you will be provided a training set and a testing set, and we will evaluate your model performance on a held out testing set.

### Project Details
First, in step imbalance, within majority classes and minority classes the instances are roughly the same, but the difference between them majority and minority can be large. Second, in linear imbalance, the different classes have different instances but the number can be coarsely interpolated linearly from smallest class to biggest class. These two imbalances are idealized from different real-world problems. The algorithm needed should be able to tackle both of them. In terms of implementation, it can be two sets of
networks or one that can distinguish the two. The evaluation metric to be used is AUROC since the traditional metric might be biased to majority class. In multi-class scenario, the ‘macro’ AUROC is used, where each metric is obtained independently for each class and then averaged among them all.

You will implement a Convolutional Neural Network technique, a manual feature extraction technique with a higher-order model (either SVM, Random Forest, or XGBoost, your choice) and linear model (logistic regression). 
