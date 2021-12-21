# Funny_muscle_enhancer :)

**1.Discription:**

1. This is just a funny project that we want to see AutoEncoder (AE) can actually work on the some features. We will start to improve...

2. Results of 1~5-times iterating  

<!-- ![image](https://github.com/JacobChen1998/Funny_muscle_enhancer/blob/main/Figure/compare.png) -->
![image](https://github.com/JacobChen1998/Funny_muscle_enhancer/blob/main/Figure/compare_version2.png)


**2.Future work:**

1. Add more data to train

2. Higher resolution

3. Imporve preprocess (Inverse_Muscle_filter.ipynb): denoise process/enhance not incude face

4. postprocess: brightness fixed/denoise process.

**3.Usage:**

1. Downloads [pre-trained model](https://drive.google.com/drive/folders/1m9JgCDnEbBIN45uC-Q-_R6hQGeRkBSNJ?usp=sharing) and put in the folder.

2. Open "Pred.ipynb" .

3. Input the image name you wwant to test.

4. Run the whole code.

**4.Training by yourself**

1. Downloads a lot of muscle image from internet (Since the copy right problem, I cannot share my dataset with you). The images type can be jpg/png/jfif/... . Notice: The more visible the muscle lines are in the images, the better. In our case, we have 204 images now.

2. Download repository-[skin detector-1](github.com/CHEREF-Mehdi/SkinDetection) and [skin detector-2](https://github.com/WillBrennan/SkinDetector). Then, put their with code.


3. Create 2 folders: before_filtering/after_filtering. Put the downloaded images in to "after_filtering" folder. Also create 2 empty folders: before_filtering_rm_bg/after_filtering_rm_bg which will load images from Inverse_Muscle_filter.ipynb

4. Run Inverse_Muscle_filter.ipynb.

5. Open training.ipynb and run the code with suitable epochs. 

**5. Update History:**

1. [2021/12/21] 
  1. Add 100+ image into dataset and remove gray style image (skin detector will not work).
  2. Modify preprocess to can output double images (weakening/original version with/without background). Original code just can output weakening/original version with background.
  3. Change training/prediction shape from (224,224,3) to (448,448,3).
  4. Training a model with size:(448,448,3) and put the new model in [pre-trained model](https://drive.google.com/drive/folders/1m9JgCDnEbBIN45uC-Q-_R6hQGeRkBSNJ?usp=sharing)
  5. Training condition as shown as following: 
  
  ![image](https://github.com/JacobChen1998/Funny_muscle_enhancer/blob/main/Figure/loss.png)
