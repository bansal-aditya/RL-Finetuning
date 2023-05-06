# 16824 Final Project

This project explores the technique of using task-specific rewards to  fine-tune pre-trained computer vision models as proposed by Pinto et al. [2023]. The fine-tuning process is posed as an RL problem, which maximizes a reward function defined based on the given task.

## The Metric Gap 

When training vision modeks, often, the loss function used to train the model may not fully align with the actual task objective. Hence, there is this gap between the model predictions and intended usage which is exacerbated for vision tasks involving complex structured outputs. 

Inspired from the domain of NLP, the above technique could circumvent the challenge of optimizing non-differentiable evaluation metrics, enabling more effcient fine-tuning of the models. 

## Reinforcement Learning 

Treat the metric  as a reward function

**REINFORCE** update rule  
$$
\theta_{t+1}=\theta_t-\eta \nabla \log (p(a \mid s)) A(s, a)
$$




## Image Superresolution

## Image Denoising 


### Model Architecture 

### Results





## References 
André Susano Pinto, Alexander Kolesnikov, Yuge Shi, Lucas Beyer, and Xiaohua Zhai. Tuning computer vision models with task rewards, 2023. URL https://arxiv.org/abs/2302.08242.