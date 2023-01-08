# Neural Networks Project

<a href="https://colab.research.google.com/drive/1FGNRza91UraR57K0O89zJTVyF6FvWtJq"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="google colab logo" height=35px></a>

[Andrea Mazzitelli](https://www.linkedin.com/in/andrea-mazzitelli/) - 1835022 - mazzitelli.1834937@studenti.uniroma1.it

[Andrea Rodriguez](https://www.linkedin.com/in/andrea-rod/) - 1834937 - rodriguez.1834937@studenti.uniroma1.it

## Introduction
This repository contains our Neural Networks Project in which we try to replicate the results obtained in the paper: [Zero Shot Image Restoration Using Denoising Diffusion Null-Space Model](https://arxiv.org/pdf/2212.00490.pdf) (Wang et al., 2022).

The paper introduces a new zero-shot approach to solve Image Restoration (IR) tasks starting from a generic pre-trained diffusion model. The authors propose a sampling algorithm called DDNM and an enhanced version DDNM+.
The method presented is Zero Shot because it can perform any IR task without needing a model explicitly trained for the task. Only a matrix representing the transformation to be done must be chosen according to the task to be performed.

In this repository you can find:
- the images used for testing;
- a pdf report containing an explanation of the method, our approach, evaluation of the results and an image gallery;
- a notebook containing the information of the report together with the code to be run.

## Instructions

To test our code open the colab, connect to a runtime with GPU and follow these instruction:

- If the colab is being executed for the first time:
  - connect to your google drive only if you want to upload custom images or masks
  - choose the parameters in the form and lauch that cell
  - run all the cells up to Algorithm implementation (it may take some minutes to download the pre-trained models)
  - choose the algorithm to use and run the corresponding cell in the Execution block
  - wait for the results that will be shown compared to the input image

- If you already run any algorithm and want to run again with some changes in the parametes:
  - change the parameters (the cell should run automatically)
  - if the changes on the parameters involved in some capacity the image or the mask (for example: changed image, added/removed the mask), run again the cell with header "Image and Mask Setup"
  - choose the algorithm to use and run the corresponding cell in the Execution block
  - wait for the results that will be shown compared to the input image

- If you want to change the model (ImageNet or CelebA):
  - change the parameters (the cell should run automatically)
  - run again the cell with header "Model Setup"
  - choose the algorithm to use and run the corresponding cell in the Execution block
  - wait for the results that will be shown compared to the input image
