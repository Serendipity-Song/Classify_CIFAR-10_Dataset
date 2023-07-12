# Classify_CIFAR-10_Dataset

This repository contains the code for a project to classify the CIFAR-10 dataset using a convolutional neural network (CNN). The project was completed using the Keras library.

## Dataset

The CIFAR-10 dataset consists of 60,000 32x32 color images in 10 classes, with 6,000 images per class. The classes are:

* Airplane
* Automobile
* Bird
* Cat
* Deer
* Dog
* Frog
* Horse
* Ship
* Truck

The dataset is split into 50,000 training images and 10,000 test images.

## Model

The model used for this project is a CNN with the following architecture:

```
Input(shape=(32, 32, 3))
Conv2D(32, kernel_size=(3, 3), activation="relu")
MaxPooling2D(pool_size=(2, 2))
Conv2D(64, kernel_size=(3, 3), activation="relu")
MaxPooling2D(pool_size=(2, 2))
Flatten()
Dense(128, activation="relu")
Dense(10, activation="softmax")
```

The model was trained using the Adam optimizer with a learning rate of 0.001. The training was stopped after 100 epochs, when the validation loss stopped decreasing.

## Results

The model achieved an accuracy of 71% on the test set. The following table shows the precision, recall, and f1-score for each class:

| Class | Precision | Recall | F1-Score |
|---|---|---|---|
| Airplane | 0.80 | 0.71 | 0.75 |
| Automobile | 0.87 | 0.74 | 0.80 |
| Bird | 0.62 | 0.60 | 0.61 |
| Cat | 0.50 | 0.56 | 0.53 |
| Deer | 0.61 | 0.72 | 0.66 |
| Dog | 0.63 | 0.62 | 0.63 |
| Frog | 0.78 | 0.82 | 0.80 |
| Horse | 0.81 | 0.73 | 0.77 |
| Ship | 0.89 | 0.74 | 0.81 |
| Truck | 0.70 | 0.86 | 0.78 |

## Conclusion

The results of this project show that it is possible to achieve a high accuracy on the CIFAR-10 dataset using a CNN. The model could be further improved by using a larger dataset, a more complex model, or a different optimizer.
<img width="507" alt="image" src="https://user-images.githubusercontent.com/88193038/236439485-52b94813-576d-4ead-8a6c-bb65fa700d3c.png">
