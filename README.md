# Gastrointestinal (GI) Tract Video Classifier
## Dataset
hyperKvasir (https://datasets.simula.no/hyper-kvasir/) <br>
* It contains 314 lower GI videos and 60 upper GI videos. <be>
* Videos have two types of resolutions - 1280 × 1024 and 720 × 576 <be>

## Preprocessing
* Frames are resized to 224 × 224 <br>

## Training
Data split <br>
- Randomly picked 60 videos from each GI <br>
    - Split: training : validation : test -> 70 : 15 : 15 <br>
    - Total training data: 84 <br>
Total validation data: 18 <br>
Total test data: 18 <br>
Loss function: Sparse Categorical Cross-Entropy <br>
Optimizer: Adam <br>
Batch size: 2 <br>
Epoch: 50 <br>







