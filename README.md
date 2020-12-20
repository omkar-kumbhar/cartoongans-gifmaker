# Cartoon GIFs using GANs

![Omkar Kumbhar](https://github.com/omkar-kumbhar/cartoongans-gifmaker/blob/main/gifs/omkar_71.gif)


![Nitesh Shinde](https://github.com/omkar-kumbhar/cartoongans-gifmaker/blob/main/gifs/nitesh_71.gif)

## Summary
- The aim of this project was to create cartoonish GIFs from real world videos using CartoonGAN.
- We trained CartoonGAN over 3000 real-world face datasets and 3000 anime faces scrapped from the web.
- Since this project deals with cartoonization, we only monitored our loss function with the focus on generator loss, and picked the best model on qualitative analysis. Inception score was not used.

## Training Progress Tracking:
For over a hundred epochs, the loss plot looks like this:
![Losses Over 100 epochs](https://github.com/omkar-kumbhar/cartoongans-gifmaker/blob/main/losses.png)

## Training Notebook
Checkout https://github.com/omkar-kumbhar/cartoongans-gifmaker/blob/main/cartoon_gans_training.ipynb

## Inference Notebook
Checkout https://github.com/omkar-kumbhar/cartoongans-gifmaker/blob/main/cartoon_gans_inference.ipynb

## GIF Maker Notebook
Checkout https://github.com/omkar-kumbhar/cartoongans-gifmaker/blob/main/cartoon_gans_gifmaker.ipynb

## Tools used
- We used Tesla V100 GPUs for training on Google Colab. 
- Framework used for training the model was pytorch.
- OpenCV was used for creating edge based features required in the model.
- Custom GIFMaker was created to convert real-world video frames to CartoonishGIFs.

## Acknowledgement
This project is inspired from CartoonGAN paper:
https://openaccess.thecvf.com/content_cvpr_2018/papers/Chen_CartoonGAN_Generative_Adversarial_CVPR_2018_paper.pdf

## Reference:
The OG Pytorch Repository:
https://github.com/znxlwm/pytorch-CartoonGAN