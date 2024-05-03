Dangerous Farm Insects Classifier

Overview

This project is developed as a part of COMP 263 at Centennial College. It focuses on utilizing deep learning to classify dangerous agricultural insects using a limited dataset. We've implemented various models including Convolutional Neural Networks (CNNs), Conditional Generative Adversarial Networks (cGANs) for data augmentation, and transfer learning with the InceptionResNetV2 architecture. Our goal is to enhance the accuracy and generalization of insect classification, which is vital for effective agricultural management.

Dataset

The dataset used in this project, known as the Dangerous Farm Insects Image Dataset, consists of 1591 high-quality images categorized into 15 classes of harmful agricultural insects. These images are primarily in RGB format, with an average resolution of 758x1015 pixels.

Models

Model 1: CNN
Architecture: Uses a sequential CNN layout with layers of convolution, max-pooling, and dense layers, integrated with L2 regularization and dropout to counteract overfitting.
Optimizer: Adam
Loss Function: Sparse Categorical Cross-entropy
Model 2: cGAN (Data Augmentation)
Purpose: To augment the training dataset with synthetically generated images, which helps in reducing overfitting and enhancing the diversity of training samples.
Model 3: Transfer Learning with InceptionResNetV2
Approach: Employs the InceptionResNetV2 architecture, pre-trained on the ImageNet dataset, to significantly improve the capability of feature extraction despite the constraints of a limited dataset size.
Results

CNN Only: Attained a training accuracy of approximately 70.9%, with a test accuracy of about 31.4%.
CNN with cGAN Augmentation: Test accuracy improved to approximately 42.7%.
InceptionResNetV2 Transfer Learning: Showed a significant enhancement with a test accuracy of approximately 79%.

Installation
git clone https://github.com/your-github-username/your-repository-name
cd your-repository-name
pip install -r requirements.txt
