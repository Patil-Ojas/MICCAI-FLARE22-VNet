# MICCAI-FLARE22-Challenge

## :gear: Overview
Required to build a 3D segmentation model for the segmentation of abdominal organs from CT scans. The primary goal is to segment the Liver, Right and Left Kidneys, and Spleen using Vnet.

## Dataset
-> CT Scans of Abdominal Organs
-> We will be focusing on Liver, Spleen, Right Kidney and Left Kidney
![image](https://github.com/user-attachments/assets/89cf8ee6-0768-41ae-86a0-ad46962128a4)

## Objective
- Train a VNet Model to segment Liver, Kidneys and Spleen
- Split the data into train and val
- Used Dice Score as eval metrics

## Setup Instructions
This is a self-contained notebook that relies solely on its own code. You can find and run the colab notebook [here](https://colab.research.google.com/drive/1fieqNqgukhR-l21fqxwOzOvx_1WeIpzM?usp=sharing).

Setting up the dataset
- Download the dataset from [here](https://zenodo.org/records/7860267).
- Upload the dataset to your Google Drive. (no need to unzip)
- Specify the path in the notebook to the zip file and the desired output location. (This may be the local colab too.)
- Execute the cells in their respective order.

- Alternavtively, you could dwonload and load the trained model from one of the links given in /main/models.
- Then define the VNet Architecture and load the model weights.
- Run predictions.

## Model Architecture
- As suggested, I have used the VNet Model Architecture from the [VNet](https://github.com/Patil-Ojas/MICCAI-FLARE22-VNet/blob/main/Papers%20Referred/Vnet_annotated.pdf) paper.
![image](https://github.com/user-attachments/assets/a2d1dd9d-9399-4164-9334-87bdf767d281)


## Training Process
- The dataset has been split in 90-10 train and val.
- You can find the detailings of all training procedures in main/logs.

## Validation and Inference
- Plotting Dice Scores vs Epochs
  
![image](https://github.com/user-attachments/assets/91ddab58-6d96-45a3-9ff2-e172df34a187)

- Also, dice score for each class was as follows
  
-> Dice score for Liver: 0.2458

-> Dice score for Right Kidney: 0.5000

-> Dice score for Spleen: 0.5000

-> Dice score for Left Kidney: 0.5000

## Video
Please Find the 2d and 3d video in main/video.

## Thank you 
- I learnt quite a bit, actually more than what I thought of. I wish I had more time to further debug the predictions.
- THank you for this challenge, it was a good one!
