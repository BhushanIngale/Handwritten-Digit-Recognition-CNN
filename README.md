
# Handwritten Digit Recognition using CNN


## Project Overview

### Problem Statement:

Correctly identify digits from a dataset of tens of thousands of handwritten images.

- Task 1: Prepare a complete data analysis report on the given data.

- Task 2: Classify a given image of a handwritten digit into one of the 10 classes representing integer values from 0 to 9.

- Task 3: Compare between various models and find the classifier that works better.

### Approach:

Classify the Images using CNNs.

## Installation & Setup

### Codes and Resources Used

- Editor/IDE: iPython Notebook on Google Colab
- Environment/Backend: TensorFlow Backend
- Python Version: 3.9

### Python Packages Used

- General Purpose: os, google.colab
- Data Wrangling: numpy
- Data Visualization: matplotlib, seaborn
- Deep Learning: tensorflow, keras

## Data
- MNIST ("Modified National Institute of Standards and Technology") is the de facto “hello world” dataset of computer vision. Since its release in 1999, this classic dataset of handwritten images has served as the basis for benchmarking classification algorithms. As new machine learning techniques emerge, MNIST remains a reliable resource for researchers and learners alike.

- Images of digits were taken from a variety of scanned documents, normalized in size, and centered. This makes it an excellent dataset for evaluating models, allowing the developer to focus on machine learning with minimal data cleaning or preparation required.

- Each image is a 28×28-pixel square (784 pixels total). A standard split of the dataset is used to evaluate and compare models, where 60,000 images are used to train a model, and a separate set of 10,000 images are used to test it.

- It is a digit recognition task. As such, there are ten digits (0 to 9) or ten classes to predict. Results are reported using prediction error, which is nothing more than the inverted classification accuracy.

Data Source: `from tensorflow.keras.datasets import mnist`

## Code Structure
```
├── data
│   └── sample_image.png
├── models
│   └── final_model.h5
├── reports
│   ├── MNIST_Report.pdf
│   └── MNIST_Report.pptx
├── src
│   ├── Handwritten-Digits-Recognition.ipynb
│   └── sample_image.png
├── .gitignore
└── README.md
```
## Results & Evaluation

| Model | Number of Layers | Learning Rate | Trainable Parameters & Size | Accuracy | Error rate |
| --- | --- | --- | --- | --- | --- |
| Simple Neural Network | 2 | 0.001 | 623290 (2.38 MB) | 0.9982 | 1.96% |
| Simple Convolutional Neural Network | 6 | 0.001 | 592074 (2.26 MB) | 0.9878 | 1.22% |
| `Modified Larger CNN` | `9` | `0.001` | `59933 (234.11 KB)` | `0.9904` | `0.77%` |

### Conclusion

We have a Convolutional Neural Network model with 9 Layers that has produced 99.04% Accuracy with the minimal error of 0.77%.

## Future Work
This model's performance can further be enhanced by tuning the Learning Rate, Model Depth and Pixel Scaling etc.

## License

[MIT](https://choosealicense.com/licenses/mit/)

