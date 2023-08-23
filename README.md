# Differentiable Learning of Quantum Circuit Born Machine
In the README.md of this repository I'll address to the Quantum Circuit Born Machine or QCBM. I will start with a brief description of th generative model and the key concept behind that. Then, I'll describe different types of allgorithems in this model with a special focus on Boltzmann Machines, Generative Adversarial Network, and Born Machines.
## Generative model 
A generative model is a type of machine learning model that aims to generate new data samples that resemble a given training dataset. The primary goal of generative models is to capture the underlying patterns, distribution, and structure of the training data in order to create new data points that are indistinguishable from real data samples. In other words, generative models learn to simulate data that is similar to what they've been trained on.

Generative models have a wide range of applications, including image synthesis, text generation, music composition, data augmentation, anomaly detection, and more. They're used whenever there's a need to generate new data points that share similar characteristics with a given dataset.

## Different types of in Generative model
There are several types of generative models, each with its own approach to generating new data. In the following I'll describe some of them 

#### Boltzmann Machines: 
A Boltzmann Machine is a type of generative model in the field of machine learning. It's a type of stochastic neural network used for unsupervised learning tasks, including generative tasks. Boltzmann Machines are designed to learn and represent the joint probability distribution of a set of binary input variables. They consist of units (neurons) that are connected with weights, and the state of each unit can be either 0 or 1. These units are organized into visible units and hidden units. The primary types of Boltzmann Machines are the Restricted Boltzmann Machine (RBM) and the Boltzmann Restricted Boltzmann Machine (BRBM). As a final word for Boltzmann Machines are less commonly used in modern applications due to the emergence of more advanced techniques such as Variational Autoencoders (VAEs) and Generative Adversarial Networks (GANs). For further information about the Boltzmann Machines I find <a href="https://github.com/yell/boltzmann-machines" target="_blank"> a useful repository </a>as agood resource. The difference between the Boltzmann Machine and Restricted Boltzmann Machines is cleared by the below graphs. 

![alt text](https://github.com/mehrankhosrojerdi/Quantum_Machine_Learning/blob/main/Boltzmann_Machine.jpg?raw=true)

#### Generative Adversarial Networks (GANs):
GANs consist of a generator and a discriminator that compete against each other. The generator tries to create realistic data samples, while the discriminator aims to distinguish between real and generated samples. This adversarial training process results in the generator creating increasingly convincing data samples.

#### Born Machines:

## Generative Adversarial Network (GAN)
Generative Adversarial Network (GAN) is a popular type of generative model. GANs consist of two main components: a generator and a discriminator. Let's break down each component and other related aspects:

Generator: The generator is a neural network that aims to generate realistic data samples that resemble the true data distribution. It takes random noise as input and produces data samples. In the context of images, for instance, if you're generating realistic human faces, the generator would produce images of faces. The goal of the generator is to improve over time by generating data that is more and more similar to the real data.

Discriminator: The discriminator is another neural network that serves as a binary classifier. It takes in both real data samples and data samples generated by the generator as inputs and tries to distinguish between them. It assigns a probability that the given input is real data. Essentially, the discriminator is like a detective trying to identify fake data.

Training Set: The training set is a collection of real data samples that your generative model will learn from. For instance, if you're generating images of cats, your training set would consist of actual images of cats.

Loss Function: The loss function is used to guide the training process. In GANs, the generator and discriminator are trained simultaneously in a competitive manner. The generator tries to minimize the discriminator's ability to differentiate between real and generated data, while the discriminator tries to maximize its ability to correctly classify real and fake data. This process results in a min-max game where the two networks are constantly improving against each other.

Training Procedure: The training procedure of a GAN involves iteratively updating the generator and discriminator networks. During each iteration, a batch of real data samples is used to train the discriminator, and another batch of random noise is used to generate fake data for training the generator. The gradients from the discriminator's loss are used to update the discriminator's weights, and the gradients from the generator's loss are used to update the generator's weights.

Hyperparameters: GANs have several hyperparameters that need to be tuned for effective training, such as learning rates, batch sizes, and network architectures. Experimenting with different hyperparameter settings can significantly impact the performance and stability of your generative model.

Evaluation: Evaluating the quality of the generated samples can be challenging. Metrics like Inception Score, Frechet Inception Distance, and visual inspection by human experts are often used to assess the quality and diversity of the generated data.

Mode Collapse: One challenge in training GANs is mode collapse, where the generator produces a limited variety of samples, ignoring certain modes in the data distribution. This can result in repetitive or low-quality outputs.

Regularization Techniques: To address issues like mode collapse and stabilize training, various regularization techniques have been proposed, such as Wasserstein GANs (WGANs), Gradient Penalty (WGAN-GP), and more.

Remember that building and training a GAN can be complex and require careful tuning. It's a fascinating area of machine learning but may take some experimentation to get the best results.
![alt text](https://github.com/mehrankhosrojerdi/Quantum_Machine_Learning/blob/main/gans_gfg.jpg?raw=true)
## QCBM



