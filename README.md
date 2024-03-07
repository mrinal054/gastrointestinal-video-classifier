# Gastrointestinal (GI) Tract Video Classifier
## Dataset
hyperKvasir (https://datasets.simula.no/hyper-kvasir/) <br>
* It contains 314 lower GI videos and 60 upper GI videos. <be>
* Videos have two types of resolutions - 1280 × 1024 and 720 × 576 <be>

## Preprocessing
* Frames are resized to 224 × 224 <br>

## Training
Data split
    * Randomly picked 60 videos from each GI
Split: training : validation : test  70 : 15 : 15
Total training data: 84
Total validation data: 18 
Total test data: 18
Loss function: Sparse Categorical Cross-Entropy
Optimizer: Adam
Batch size: 2
Epoch: 50
![image](https://github.com/mrinal054/gastrointestinal-video-classifier/assets/44781227/cfd4950f-a92d-40d0-b604-3296bb1dbfc1)






