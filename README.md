# 👁️ Kidney Condition Analysis Through Iris

**An experimental computer vision and machine learning project for iris image processing and normal/abnormal classification to detect kidney condition.**

This project explores an image-analysis workflow using Python and computer vision techniques to process eye images, extract regions of interest (ROI), analyze pixel distributions, and classify images into normal and abnormal categories.

> **Research disclaimer:** This is an academic experimental project. Iris-image classification has not been established here as a clinically validated method for diagnosing kidney disease. The results must not be used for medical diagnosis or treatment decisions.

## 📌 Project Overview

The project investigates whether image-processing and machine-learning techniques can be applied to iris images for exploratory analysis of potential cardiovascular and renal health indicators.

The workflow includes image enhancement, preprocessing, iris-region extraction, histogram analysis, ROI analysis, and classification.

### ✨ Key Features

- **Image preprocessing:** Median filtering and image sharpening.
- **Color analysis:** RGB-based sclera color recognition.
- **Automatic cropping:** Identifies and crops the relevant iris region.
- **Edge detection:** Applies the Sobel operator to highlight image boundaries.
- **Feature analysis:** Examines black and white pixel distributions within a selected region of interest.
- **Classification:** Explores normal/abnormal image classification using the method implemented in the notebook.
- **Google Colab:** Supports experimentation in a notebook-based Python environment.

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| Python | Main programming language |
| OpenCV | Image processing and computer vision |
| NumPy | Numerical and pixel-array operations |
| Pandas | Data handling and analysis |
| Matplotlib | Visualization of image-processing results |
| Google Colab | Notebook execution and experimentation |

## 🔄 Project Workflow

1. **Image acquisition:** Load the available normal and abnormal eye-image samples.
2. **Image enhancement:** Apply sharpening and median filtering.
3. **Preprocessing:** Process image colors and convert pixels into a suitable representation.
4. **Iris extraction:** Use histogram projections and automatic cropping to isolate the relevant region.
5. **Edge detection:** Apply Sobel edge detection to highlight image structures.
6. **ROI analysis:** Calculate pixel-based features from the selected region.
7. **Classification:** Apply the implemented thresholding or trained classification model.
8. **Result visualization:** Display the processed images and classification output.

## 🧠 Classification Approach

The project report describes Support Vector Machine (SVM) as a classification approach. The research paper also discusses threshold-based classification using the ratio of black and white pixels in the selected ROI.

The reported threshold rule describes an image as normal when the average white-pixel ratio is below 0.275 and the black-pixel ratio is above 0.725; other cases are categorized as abnormal.

## 🚀 Getting Started

### Run in Google Colab

1. Open the original notebook in Google Colab.
2. Ensure that the dataset paths and Google Drive permissions are configured correctly.
3. Select **Runtime → Run all**.
4. Review the preprocessing, ROI extraction, and classification outputs.

[Open the Google Colab notebook]
https://colab.research.google.com/drive/1GUEpVEhOxO-kK5mO2pQFoa79gQrf4Fn7?usp=sharing


## 📊 Results and Evaluation

- By analyzing specific features extracted from eye images, including iris and sclera regions, as well as utilizing histogram analysis for heart region of interest (ROI), we aimed to identify abnormalities indicative of potential heart diseases and kidney problems. Our methodology involves image preprocessing, feature extraction, and thresholdbased classification, offering a non-invasive and cost-effective means of screening for cardiovascular health issues. 
- Our proposed approach demonstrated promising results in terms of accuracy in distinguishing between normal and abnormal cases. 
- This research contributes to the growing body of literature on non-invasive cardiovascular and renal  methods for health prediction.  
- Ultimately, this research could lead to early detection and prevention of cardiovascular and renal diseases, benefiting public health .

## 🔮 Future Improvements

- Evaluate SVM against other suitable classification methods.
- Improve iris segmentation and feature extraction.
- Add reproducible model evaluation and error analysis.
- Test on an appropriately sourced, documented, and independently evaluated dataset.
- Build a Streamlit interface for uploading images and viewing experimental processing results.
