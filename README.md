Project Title: AI-Based Handwritten Digit Generation Using Generative Adversarial Networks


Problem Statement

Generative AI can be used to create new images that resemble real-world data. In this project, students will build a Generative Adversarial Network (GAN) using TensorFlow/Keras to generate handwritten digit images similar to the MNIST dataset.

The project focuses on understanding how a Generator and Discriminator work together, training an adversarial model, and evaluating the quality of generated images.

Objective

Understand the basic concept of Generative AI and GANs.

Preprocess the MNIST image dataset.

Build Generator and Discriminator networks.

Train a GAN using adversarial learning.

Generate new handwritten digit images.

Analyze GAN training using generated images and loss curves.

Dataset: MNIST dataset available directly through TensorFlow/Keras.






Task Description:

You are required to:

Build and train a GAN model using TensorFlow 2.x (Keras API) consisting of:

Generator Network: Takes a random noise vector (e.g., 100-dimensional) and outputs a 28×28 grayscale image. 

Discriminator Network: Classifies input images (real or generated) as true (1) or fake (0).

Dataset: Use the MNIST dataset available in TensorFlow:

(x_train, _), (_, _) = tf.keras.datasets.mnist.load_data()

Normalize the data to the range [-1, 1] and reshape to (28, 28, 1).

Model Design Guidelines:

 Generator:
 
 Layers: Dense → BatchNormalization → LeakyReLU → Conv2DTranspose → Output (Tanh)
 
Discriminator:

 Layers: Conv2D → LeakyReLU → Dropout → Flatten → Dense (Sigmoid)
 
 Loss Function: Binary Cross-Entropy (BCE)
 
 Optimizer: Adam (learning rate = 0.0002, β1 = 0.5).
 
 Train for at least 20 epochs and visualize the progress.
 
Output Requirement:

 Display a grid of generated digit images every few epochs.
 
 Plot loss curves for the generator and discriminator.
 



Deliverables

Submit the complete project through GitHub. The repository must contain:

Jupyter Notebook (.ipynb) with code and outputs

Dataset details

GAN preprocessing

Generator implementation

Discriminator implementation

Training implementation

Generated image samples

Generator and Discriminator loss graphs
README.md 
