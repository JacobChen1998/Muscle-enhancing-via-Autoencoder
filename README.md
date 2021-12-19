# Funny_muscle_enhancer

**1.Discription:**

 This is just a funny project that we want to see AutoEncoder (AE) can actually work on the some features. We will start to improve...


**2.Future work:**

1. Add more data to train

2. Higher resolution

**3.Usage:**

1. Downloads model from [link](https://drive.google.com/drive/folders/1m9JgCDnEbBIN45uC-Q-_R6hQGeRkBSNJ?usp=sharing) and put in the folder.

2.Open "Pred.ipynb" .

3.Input the image name you wwant to test.

4.Run the whole code.

**4.Training by yourself**

1. Downloads a lot of muscle image from internet (Since the copy right problem, I cannot share my dataset with you). The images type can be jpg/png/jfif/... . Notice: The more visible the muscle lines are in the images, the better. In our case, we have 204 images now.

2. Create 2 folders: before_filtering/after_filtering. Put the downloaded images in to "after_filtering" folder.

3. Run Inverse_Muscle_filter.ipynb.

4. Open training.ipynb and run the code with suitable epochs. In our case, we trained with 175 epochs.
