# Generative Adversarial Networks (GANs) for CIFAR-10 Image Generation

## Project Structure

- **`gan_cifar10.ipynb`**: Contains code to define the Generator and Discriminator models, train the GAN on the CIFAR-10 dataset, and visualize the generated images.
- **`data/cifar10.npz`**: The CIFAR-10 dataset in NumPy's `.npz` format, used for training.
- **`model/cifar_generator.h5`**: The Generator model saved after 1000 epochs of training.

## How to Use

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/gan-cifar10.git
cd gan-cifar10
```

### 2. Install Dependencies
Ensure you have Python 3 and the following libraries installed:

```bash
pip install numpy keras matplotlib pandas
```

### 3. Run the Jupyter Notebook
- Launch Jupyter Notebook:
```bash
jupyter notebook
```
- Open gan_cifar10.ipynb and run all cells to see the training process and generated images.
- **Note:** Training the GAN from scratch can be time-consuming. If you prefer to use the pretrained model:
    - Skip to the section where the model is loaded:
    ```bash
    model = load_model('models/cifar_generator.h5')
    ```
    - Generate and visualize images using the pretrained Generator.

## Model Training

The model was trained for ``1000 epochs`` using Kaggle's GPU environment. While increasing the number of epochs may yield better results, Kaggle's resource limitations influenced the choice of 1000 epochs. Training for more epochs on a local machine or more powerful environment may improve the quality of generated images.`

## Results
After 1000 epochs, the Generator can produce images that resemble those in the CIFAR-10 dataset. The generated images can be visualized using the provided notebook, which displays them in a grid format for easy assessment.