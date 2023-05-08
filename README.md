# 16824 Final Project

This project explores the technique of using task-specific rewards to  fine-tune pre-trained computer vision models as proposed by Pinto et al. [2023]. The fine-tuning process is posed as an RL problem, which maximizes a reward function defined based on the given task.

## The Metric Gap 

When training vision models, often, the loss function used to train the model may not fully align with the actual task objective. Hence, there is this gap between the model predictions and intended usage which is exacerbated for vision tasks involving complex structured outputs. 

Inspired from the domain of NLP, the above technique could circumvent the challenge of optimizing non-differentiable evaluation metrics, enabling more efficient fine-tuning of the models. 

## Reinforcement Learning 
Treat the metric  as a reward function

**REINFORCE** update rule  

![reinforce](https://user-images.githubusercontent.com/12653676/236592832-e4aaab91-b03a-4224-94c3-e3ff70a49abe.png)


![rl](https://user-images.githubusercontent.com/12653676/236592930-f448946f-3a8d-4d14-9f9e-05df40d09f60.png)


## Image Super-Resolution

This is a standard task in computer vision, where one attempts to increase the resolution of images. The task is typically formulated as a conditional image generation problem, where the input is a low-resolution image and the output is a high-resolution image

### Model Architecture 

![srflow_arch](https://user-images.githubusercontent.com/12653676/236910846-8eccf91b-0269-4b9f-b953-a5727fcbedec.png)

### Result Images

<img width="521" alt="Screenshot 2023-05-08 at 3 05 33 PM" src="https://user-images.githubusercontent.com/12653676/236910572-26344ec5-41af-45b4-ab9b-21fdf8ccf75d.png">

## Image Denoising 

Image denoising is the task of removing noise or unwanted distortions from an image, which is usually the result of random variations in the image signal caused by factors such as low light conditions,
imperfect camera sensors, or transmission errors in the image acquisition proces

### Model Architecture 

![rdunet](https://user-images.githubusercontent.com/12653676/236593325-bcc9bd85-1ede-48fd-8f77-9d1ebf1b02be.png)

### Result Images

<img width="598" alt="all_denoise" src="https://user-images.githubusercontent.com/12653676/236706335-f8e1b1fe-b51a-4359-a8e5-08154ac287e5.png">

## References 
André Susano Pinto, Alexander Kolesnikov, Yuge Shi, Lucas Beyer, and Xiaohua Zhai. Tuning computer vision models with task rewards, 2023. URL https://arxiv.org/abs/2302.08242.
