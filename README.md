# YOLOV11-Search-App

## ABSTRACT

YOLOV11 Search App is a Streamlit based image search application that uses YOLOV11 object detection to analyze images and create a searchable gallery. It detects objects, stores results as JSON metadata, and lets users search images by object classes (e.g., person, car, apple, bat). Users can filter images containing single or multiple objects and control object count for quick dataset exploration and computer vision demos.

---

## Use Cases

This project helps answer questions like:

- Which images contain a bat?
- Which images contain an apple or a baseball bat?
- Which images contain all selected objects?
- Which images contain a selected object within a chosen count limit?

---

## Model Information

This project uses the COCO dataset classes, containing 80 common object categories such as:

- Person
- Car
- Dog
- Cat
- Airplane
- Banana

The detection model used is YOLOV11, chosen for its:

- Fast inference speed
- Improved detection accuracy
- Real-time object detection capability

The model predicts:

- Object Classes
- Bounding Boxes
- Confidence Scores

These predictions are converted into searchable metadata for efficient image retrieval.

---

# Environment Setup

### Requirements

- Python 3.11
- Anaconda / Miniconda
- Visual Studio Code (VS Code)
- NVIDIA GPU (Optional — for GPU acceleration)

---

# Required Project Files

```text
requirements.txt
instructions.txt
app.py
```

---

# GPU Installation Steps

## Step 1 — Create Conda Environment

```bash
conda create -n yolo-image-search-gpu python=3.11 -y
```

## Step 2 — Activate Environment

```bash
conda activate yolo-image-search-gpu
```

## Step 3 — Install PyTorch with CUDA Support

```bash
conda install pytorch torchvision pytorch-cuda=12.4 -c pytorch -c nvidia
```

## Step 4 — Install Project Dependencies

```bash
pip install -r requirements.txt
```

---

# How to Run in VS Code using Conda

## Activate Environment

```bash
conda activate yolo-image-search-gpu
```

## Launch the Streamlit Interface

```bash
streamlit run app.py
```

---

# Browser URL

```text
Local URL: http://localhost:8501
```

This will automatically open the Streamlit app in your browser.

# OUTPUT
## UI SCREENSHOT
<img width="1023" height="424" alt="image" src="https://github.com/user-attachments/assets/24642758-b702-4ab9-8826-5e942a5d58f5" />

## DETECTION
<img width="1008" height="445" alt="image" src="https://github.com/user-attachments/assets/8e1e85e5-46bb-47d7-aa60-02b72e200036" />
<img width="1029" height="303" alt="image" src="https://github.com/user-attachments/assets/ccf4d3e1-8b96-4ecc-964f-379755dcd66c" />

## RESULT
The YOLO Image Search System successfully performs object detection, metadata generation, and image retrieval using YOLOv11.



