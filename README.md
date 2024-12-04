# Brain MRI Reconstruction with 3D Convolutional Autoencoder

This project focuses on the reconstruction of brain MRI images using a 3D Convolutional Autoencoder (CAE) implemented in TensorFlow/Keras. The goal is to accurately reconstruct healthy brain MRIs and evaluate the performance of the model across various datasets, including healthy controls, patients with Mild Cognitive Impairment (MCI), and patients with Alzheimer’s Disease (AD).

## Features
- **Data Preprocessing**: CLAHE equalization, intensity normalization, reorientation, and resizing of MRI scans.
- **Model Architecture**: U-Net inspired 3D Convolutional Autoencoder.
- **Training**: Configured with Early Stopping, Model Checkpointing, and ReduceLROnPlateau.
- **Evaluation**: MSE and SSIM metrics used for performance evaluation on various datasets.
- **Visualization**: Interactive tools for visualizing original, reconstructed images, and error heatmaps.

## Prerequisites

Ensure you have Python 3.x and the following libraries installed:

```bash
pip install -r requirements.txt

Due to file size limitations, the trained model and datasets cannot be provided with this repository. Consequently, you will not be able to execute the code directly unless you have access to the required data files. However, if the necessary data and model files were available, here’s how you would work with the provided Jupyter Notebook:

Open the Jupyter Notebook
Launch Jupyter Notebook in your project directory and open the .ipynb file.

Set Up the Environment
Run the first code block to import all necessary libraries.

Load and Preprocess Data
Execute the code blocks that load and preprocess the MRI datasets. These blocks typically follow the import statements.
Ensure the paths to the datasets are correctly specified according to your local file structure.

Define the Model
Run the code block that defines the 3D Convolutional Autoencoder (CAE) model using TensorFlow/Keras.

Train the Model
Execute the training code block, which configures and trains the CAE. This will include setting up callbacks like EarlyStopping and ModelCheckpoint.
The model will train for a specified number of epochs, and checkpoints will save the best model based on validation performance.

Evaluate the Model
After training, run the evaluation code blocks to assess the model's performance using MSE and SSIM metrics on the test datasets.

Visualize Results
Finally, execute the visualization blocks to view original vs. reconstructed images and the corresponding error heatmaps. This section includes interactive tools for detailed inspection.
