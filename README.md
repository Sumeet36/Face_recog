# Face_recog
## Face recognition system (vgg16)

### Step 1:  Collecting the Dataset

The first step before training any model is collecting the dataset.

In this project I have used cv2 to collect the dataset - it uses the camera of the laptop to take pictures of your face and stores them in the specified directory.

I have collected the images of my face and my sister's face for the dataset. So I have 2 classes.

I collected 1000 images for each class and then I manually splitted them into 2 folders - train and validation.

The Training and Testing dataset can be splitted in any ratio. Here, I splitted it in ratio 8:2.

### Step 2: Training Model

After collecting the dataset , we used a pre-trained model - of which all the convolution layers are freezed and new dense / fully connected layers are added which are then trained for the dataset collected previously.

### Step 3: Saving the Model

The trained model is then saved.

This saved model can be loaded at any point of time in any file to predict the results.

### Step 4: Predicting Results

To predict the results and check if the model is working fine or not. You can either use a photo that you have clicked or you can use your camera to predict the face in real time. In my case, I used my camera to take a picture of mine and then predicted the result.
Since I only had two classes so I wrote a simple python code with if else conditions, but if you have more than 2 classes, you can change the pyhton code according to your requirements.
