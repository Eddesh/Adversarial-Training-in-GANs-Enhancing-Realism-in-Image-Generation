# Adversarial-Training-in-GANs-Enhancing-Realism-in-Image-Generation

## Project Overview
This project explores the use of Generative Adversarial Networks (GANs) for generating realistic images. GANs consist of two neural networks, a Generator and a Discriminator, that engage in an adversarial game. This project demonstrates how these networks are trained together, enhancing the Generator's ability to produce images indistinguishable from real data. We measure the performance using the Fréchet Inception Distance (FID), which helps evaluate the similarity between generated images and real images.

### Dataset Description
The dataset includes a variety of labeled images used for training and evaluation. For the purpose of generating realistic images, specific classes from the dataset were chosen. Key aspects of the dataset include:
- Labels: Class labels indicating the category of each image.
- Grayscale Images: The images were converted to grayscale and normalized to enhance stability during GAN training.
- Training and Testing: The data is split for training and testing, allowing for robust evaluation of the generated images’ realism.

### Step 1: Model Training
- The Adversarial Training in GANs Enhancing Realism in Image Generation.ipynb notebook contains the code for data preprocessing, model training, and evaluation. Both the Generator and Discriminator are trained in an adversarial manner.
- The training process involves using random noise as input to the Generator, which produces synthetic images. The Discriminator evaluates these images against real images to improve the Generator's outputs.
### Step 2: Image Generation
- Once the model is trained, it can be used to generate images. You can modify the noise vector to control the output characteristics.
- Execute the cells in the notebook to observe generated images and evaluate them using FID.
### Step 3: Evaluation
- This project uses the Fréchet Inception Distance (FID) to assess the quality of generated images. A lower FID score indicates that the generated images are more realistic and similar to the real dataset.
- To compute FID, the project includes functions for extracting features and comparing distributions.

### Testing
The project was evaluated with FID at different training stages:

### Stages
1. Early Stage (Epoch 5): The Generator begins producing basic shapes but lacks detail.
2. Mid Stage (Epoch 100): Generated images become more defined and realistic.
3. Late Stage (Epoch 200): The images exhibit high realism, approaching the quality of real images in terms of structure and detail.
4. Each stage highlights the progressive improvement in image quality. The FID scores at various epochs indicate the Generator’s increasing capability to mimic real data.

![image](https://github.com/user-attachments/assets/0c3d5f3a-3143-4564-8c5f-e53b7121f8ec)
![image](https://github.com/user-attachments/assets/21b7d922-9aff-40e3-849a-2bdef2f0ed7e)

## Author
Davin Edbert Santoso Halim
