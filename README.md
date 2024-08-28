# Line2Live


## Introduction

**Line2Live** is a Pix2pix-Based Stacked Triple-Generator Conditional Neural Network designed to transform sketches into realistic face photos. This project leverages advanced deep-learning techniques to bridge the gap between artistic sketches and lifelike facial reconstructions. The overall reconstruction quality improved by 25.1% in L1 distance, 16.2% in L2 distance, and 3.2% in Structural Similarity Index compared to the traditional pix2pix model. 

## Folder Descriptions

- **Discriminators**: where discriminators will be saved per customized number of epochs after training
- **Generator**: where generators will be saved per customized number of epochs after training
- **Final_Generation**: where test faces are produced with input sketches 
- **History & History_plots**: data and plots for saving training and validation curves
- **Sketch_Photo_Dataset**: directory for input sketches, target photos, grayscale versions of images and augmented images
- **train/validation_gen_examples**: directory where sample training and validation photos will be saved for monitoring reconstruction progress

## File Descriptions
- **config.py**: setup the configurations and type of transformations for data-preprocessing for entire training
- **dataset.py & dataset_multi.py** customized datasets for loading multi images simultaneously
- **discriminator.py**: discriminator model class
- **generator.py**: generator model class
- **metric_evaluation**: evaluate the L1, L2 distance and SSIM based on images generated saved in Final_Generation folder with input test sketches
- **utils.py**: some helper functions for image saving and model loading

## Usage

To get started with Line2Live, follow these steps to set up the project on your local machine.

```bash
# Clone the repository
git clone https://github.com/angel-gao/Line2Live.git

# Install dependencies
conda env create -f environment.yml
```

To run the 

