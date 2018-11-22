# CCU-Final-Project

**Producing 256*256 output images with 2000 epochs, your code should be implemented as below ↓**

**Execute:** CUDA_VISIBLE_DEVICES='0' python train_conditional_wgan.py --dataset Clothes_Final/
 --width 256 --height 256 channels 3 --z_dim 100 --batch_size 8 --epochs 2000 --preview_iteration 693 --std 1.0
 
 **Produce Output:** CUDA_VISIBLE_DEVICES='2' python3 inference_acgan.py TEST/ Logo  tags.csv --model weights128x128-1.h5 --batch_size 1 --std 0.8 --n 100
---
**Instructions:**

**CUDA_VISIBLE_DEVICES='0'** → Means to use GPU='0'

**--dataset Clothes_Final/** → Implement your dataset (Ex: Clothes_Final/)

**--width 256 --height 256** → Output resolution (Ex: 256*256)

**channels 3** → Input color RGB

**--z_dim 100** → Sampling from 100 dimension's normal distribution

**--batch_size 8** → 


