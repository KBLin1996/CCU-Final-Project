# CCU Final Project

**To produce 256*256 output images with 3000 epochs, your code should be implemented as below ↓**

**DataSet:** https://drive.google.com/drive/folders/1G3q5rrmCao5kboao904vhaSjsVr_O4Vi?usp=sharing

**Execute:** CUDA_VISIBLE_DEVICES='0' python train_wgan.py --dataset Clothes_Final/
 --width 256 --height 256 channels 3 --z_dim 100 --batch_size 8 --epochs 3000 --preview_iteration 693 --std 1.0
 
 **Produce Output:** CUDA_VISIBLE_DEVICES='0' python3 acgan.py TEST/ Logo/  tags.csv --model weights128x128-1.h5 --batch_size 1 --std 0.8 --n 100
 
---

**Instructions in Execute:**

**CUDA_VISIBLE_DEVICES='0'** → Means to use GPU='0'

**--dataset Clothes_Final/** → Implement your dataset (Ex: Clothes_Final/)

**--width 256 --height 256** → Output resolution (Ex: 256*256)

**channels 3** → Input color RGB

**--z_dim 100** → Sampling from 100 dimension's normal distribution

**--batch_size 8** → Batch size (How many images a batch)

**--epochs 3000** → Epochs (Run how many times)

**--preview_iteration 693** → How many batchs preview once
 
---

**Instructions in Produce Output:**

**TEST/** → Your output directory's destination

**Logo/** → What catagory do you want to produce

**--model weights128x128-1.h5** → Your .h5 file (Located in a directory called "Preview_Project")

**--std 0.8** → How blur is your ouput images (From 0~1)

---

**Discriminator Structure**

![image](https://github.com/KBLin1996/CCU-Final-Project/blob/master/Discriminator.PNG)

**Generator Structure**

![image](https://github.com/KBLin1996/CCU-Final-Project/blob/master/Generator.PNG)

---

**Result (Epoch 300)**

![image](https://github.com/KBLin1996/CCU-Final-Project/blob/master/Epoch300.PNG)

**Result (Epoch 400)**

![image](https://github.com/KBLin1996/CCU-Final-Project/blob/master/Epoch400.PNG)

---

**Training Loss**

![image](https://github.com/KBLin1996/CCU-Final-Project/blob/master/Loss.PNG)
