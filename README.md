# Deep-Learning-Assignment2
CNN | RNN Variants | Generative Adversarial Networks
Course: Deep Learning (IS3332-1)
Student: Deviprasad
USN: NNM23IS047
Section & Semester: 6th A
Institution: NMAM Institute of Technology, Nitte
Submitted To: Dr. Jason Elroy Martis, Associate Professor
Date: 23-03-2026

📌 Overview
This repository contains the implementation of three deep learning models as part of Assignment 2:
TaskModelDatasetImage ClassificationCustom CNN + ResNet18 (Transfer Learning)MNISTSentiment ClassificationRNN, LSTM, GRUIMDB Movie ReviewsImage GenerationGenerative Adversarial Network (GAN)Fashion-MNIST

📂 Repository Structure
Deep-Learning-Assignment2/
│
├── Deviprasad_NNM23IS047_DL_task2.ipynb   # Main Colab Notebook (all 3 tasks)
└── README.md                               # Project documentation

🚀 How to Run

Click the Open in Colab button below
Go to Runtime → Run All
All models will train and display results automatically

Show Image

🧠 Models Implemented
Task A — Convolutional Neural Network (CNN)

Custom CNN with 2 convolutional blocks, Batch Normalisation, Dropout
Transfer Learning using pretrained ResNet18 (modified for grayscale MNIST input)
Dataset: MNIST (70,000 handwritten digit images, 10 classes: 0–9)

ModelTest AccuracyCustom CNN99.1%ResNet18 (Transfer Learning)95.3%

Custom CNN outperformed ResNet18 because MNIST's simple 28×28 grayscale digit patterns
are better suited to a lightweight task-specific architecture than a large ImageNet-pretrained model.


Task B — Recurrent Neural Networks

Simple RNN, LSTM, and GRU for binary sentiment classification
Dataset: IMDB Movie Reviews (50,000 reviews, Positive / Negative)

ModelTest AccuracySimple RNN80.3%LSTM84.8%GRU85.9%

GRU achieved the best accuracy with fewer parameters than LSTM,
making it the most efficient model for this task.


Task C — Generative Adversarial Network (GAN)

Generator: 3 Dense layers → produces 28×28 clothing images from random noise
Discriminator: 2 Dense layers → classifies real vs fake images
Dataset: Fashion-MNIST
Trained for 30 epochs — discriminator accuracy stabilised at ~50%


🛠️ Technologies Used

Python 3.x
PyTorch (CNN, ResNet18)
TensorFlow / Keras (RNN, LSTM, GRU, GAN)
Torchvision
Matplotlib, Seaborn
Scikit-learn
Google Colab (GPU)


📊 Key Results

Custom CNN achieved 99.1% accuracy on MNIST — near perfect classification
GRU achieved the best accuracy (85.9%) among all recurrent models
GAN successfully generated recognisable Fashion-MNIST clothing images after adversarial training
Discriminator accuracy converging to ~50% confirms stable GAN equilibrium


📁 Dataset Sources

MNIST Dataset
IMDB Dataset
Fashion-MNIST


📚 References

Goodfellow et al., Deep Learning, MIT Press, 2016
LeCun et al., The MNIST Database of Handwritten Digits, 1998
PyTorch Documentation — https://pytorch.org/docs/
TensorFlow Documentation — https://www.tensorflow.org/


📝 Academic Integrity
This assignment is my own original work submitted as part of the Deep Learning course (IS3332-1) at NMAM Institute of Technology, Nitte.
