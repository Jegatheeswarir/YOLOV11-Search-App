# YOLOV11-Search-App

# ABSTARCT
YOLOV11 Search App is a Streamlit-based image search application that uses YOLOv11 object detection to analyze images and create a searchable gallery. It detects objects, stores results as JSON metadata, and lets users search images by object classes (e.g., person, car, apple, bed). Users can filter images containing single or multiple objects and control object count for quick dataset exploration and computer vision demos.
## Use Cases

This project helps answer questions like:

 Which images contain a bed?
 Which images contain an apple or a baseball bat?
 Which images contain all selected objects?
 Which images contain a selected object within a chosen count limit?

##  Model Information

This project uses the COCO dataset classes, containing 80 common object categories such as:

Person
Car
Dog
Cat
Airplane
Banana

The detection model used is YOLOv11, chosen for its:

Fast inference speed
Improved detection accuracy
Real-time object detection capability

The model predicts:

Object Classes
Bounding Boxes
Confidence Scores
These predictions are converted into searchable metadata for efficient image retrieval.

# EnvironmentSetup
Python 3.11
Anaconda / Miniconda
Visual Studio Code (VS Code)
NVIDIA GPU (Optional – for GPU acceleration)

# Required project files:
```
requirements.txt
instructions.txt
app.py
```
# GPU Installation Steps
## Step 1 – Create Conda Environment
```
conda create -n yolo-image-search-gpu python=3.11 -y
```
## Step 2 – Activate Environment
```
conda activate yolo-image-search-gpu
```
## Step 3 – Install PyTorch with CUDA Support
```
conda install pytorch torchvision pytorch-cuda=12.4 -c pytorch -c nvidia
```
## Step 4 – Install Project Dependencies
```
pip install -r requirements.txt
```
# How to Run in VS Code using Conda
## Activate Environment
```
conda activate yolo-image-search-gpu
```
## Launch the Streamlit interface
```
streamlit run app.py
```
## The terminal will display and Open Browser:
```
Local URL: http://localhost:8501
```
# OUTPUT
## UI Screenshot
<img width="1219" height="576" alt="image" src="https://github.com/user-attachments/assets/8ee8a344-1d02-4109-8711-b99d6fe7c44b" />

## Object Detection Output
<img width="1818" height="802" alt="image" src="https://github.com/user-attachments/assets/7fa196cf-2d3f-4abd-ae66-6620252255e2" />
<img width="1709" height="521" alt="image" src="https://github.com/user-attachments/assets/9f9faf94-6d92-4045-ad64-96bb37596564" />
<img width="1812" height="518" alt="image" src="https://github.com/user-attachments/assets/b7621d1f-a1e1-410e-a6d3-b036dbd8e0ad" />


# RESULT
The YOLO Image Search System successfully performs object detection, metadata generation, and image retrieval using YOLOv11.
