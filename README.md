# CCU Final Project

**Overall: Implement a model that used WGAN to generate man's clothes by itself**

***Clothes DataSet Download:** https://drive.google.com/drive/folders/1G3q5rrmCao5kboao904vhaSjsVr_O4Vi?usp=sharing*

**Reference:** https://github.com/peter0749/WGAN-GP-Anime-with-Auxiliary-Classifier

---

**To produce 256*256 output images with 4000 epochs, your code should be implemented as below ↓**

**Execute:** CUDA_VISIBLE_DEVICES='0' python train_wgan.py --dataset Clothes_Final/
 --width 256 --height 256 channels 3 --z_dim 100 --batch_size 8 --epochs 4000 --preview_iteration 693 --std 1.0
 
**Produce Output (Create new clothes in directory "Final"):** CUDA_VISIBLE_DEVICES='0' python3 output.py Final/ Logo tags.csv --model weights128x128-1.h5 --batch_size 1 --std 0.8 --n 100
 
---

**Instructions in Execute:**

**CUDA_VISIBLE_DEVICES='0'** → Means to use GPU='0'

**--dataset Clothes_Final/** → Implement your dataset (Ex: Clothes_Final/)

**--width 256 --height 256** → Output resolution (Ex: 256*256)

**channels 3** → Input color RGB

**--z_dim 100** → Sampling from 100 dimension's normal distribution

**--batch_size 8** → Batch size (How many images a batch)

**--epochs 4000** → Epochs (Run how many times)

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

**Result (Epoch 400)**

![image](https://github.com/KBLin1996/CCU-Final-Project/blob/master/Epoch400.PNG)

**Result (Epoch 2900)**

![image](https://github.com/KBLin1996/CCU-Final-Project/blob/master/Epoch%202900.jpg)

**Result (Epoch 3094)**

![image](https://github.com/KBLin1996/CCU-Final-Project_WGAN/blob/master/Epoch3094.jpg)

**Result (Epoch 1 ~ 3100, Preview Variety)**

![image](https://github.com/KBLin1996/CCU-Final-Project_WGAN/blob/master/1~3100Epochs.gif)

---

**Training Loss**

![image](https://github.com/KBLin1996/CCU-Final-Project/blob/master/Loss.PNG)
