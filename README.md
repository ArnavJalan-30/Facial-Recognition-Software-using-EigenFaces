# Eigenfaces for Facial Recognition

This repository contains the files for our group project based on the paper "Eigenfaces for Recognition" by Matthew Turk and Alex Pentland. The project implements a face recognition system using eigenfaces, a technique that uses Principal Component Analysis (PCA) to recognize faces by reducing dimensionality and representing faces with fewer key features.

## Group Members
- Arnav Aditya [2210110189]
- Arnav Jalan [2210110192]
- Aditya Raghuram [2210110126]
- Naman Singhal [2210110986]

## Project Overview

Face recognition plays a crucial role in applications such as security systems, human-computer interaction, and biometric identification. This project builds on the **Eigenfaces** method, which breaks down face images into a set of characteristic "eigenfaces" and compares new images with these stored features for recognition. 

Our approach follows the core ideas in the original paper:
1. **Data Collection**: Gathering grayscale face images.
2. **Preprocessing**: Noise reduction, normalization, and alignment.
3. **Dimensionality Reduction**: Using PCA to compute eigenfaces from the dataset.
4. **Recognition**: Projecting input images into the eigenspace and using distance metrics (e.g., Euclidean distance) to classify them.

## Tech Stack
- **Python**: 3.10.6
- **Jupyter Notebook**: 6.5.4
- **NumPy**: 1.24.3
- **Matplotlib**: 3.7
- **Operating System**: Linux (Virtual Machine)

## Project Workflow

### 1. Setup Instructions
1. Install Python, Jupyter, Matplotlib, and NumPy using your preferred method.
2. Ensure that the following versions are installed:
   - Python: 3.10.6
   - Jupyter Notebook: 6.5.4
   - NumPy: 1.24.3
   - Matplotlib: 3.7
3. Clone this repository and open the Jupyter notebook `Eigenfaces_for_recognition.ipynb`.
4. Place the dataset in the same folder as the notebook.

### 2. Running the Project
1. Open the notebook in Jupyter.
2. Ensure that all required libraries are installed (`NumPy`, `Matplotlib`, etc.).
3. Load the dataset and run each cell in the notebook sequentially.
4. The cells will:
   - Preprocess the images.
   - Compute eigenfaces using PCA.
   - Perform face recognition on test images.
   
### 3. Eigenfaces Method
- **Preprocessing**: Filters are applied to reduce noise, normalize lighting, and align facial features.
- **Principal Component Analysis (PCA)**: PCA reduces the dataset’s dimensionality, generating eigenfaces that represent the most significant facial features.
- **Face Recognition**: New faces are projected into the eigenspace spanned by the eigenfaces, and their positions are compared to recognize the face.

## Key Results
- The project successfully implements facial recognition with eigenfaces.
- Mean face, normalized faces, and eigenfaces are computed and visualized.
- Recognition accuracy and examples of correctly recognized faces are shown in the notebook.

## Limitations
- **Background Influence**: Background noise affects recognition performance. We applied Gaussian windows to reduce the impact.
- **Pose & Scale Sensitivity**: Recognition accuracy diminishes with changes in head size and orientation. Multi-scale approaches and input scaling partially resolve this issue.
- **Lighting Conditions**: The algorithm’s performance can degrade under varied lighting conditions.
- **Computational Intensity**: PCA with large datasets can be computationally expensive.

## Learning Outcomes
This project provided insight into facial recognition using eigenfaces and PCA. We learned:
- How eigenfaces efficiently reduce the complexity of face recognition.
- The importance of dimensionality reduction in handling large datasets.
- Challenges posed by lighting, background, and pose variations in face recognition tasks.

## Acknowledgments
We thank Professor Santosh Singh for guiding us through this project and helping us understand key concepts in linear algebra, particularly eigenvalues and eigenvectors.

## Bibliography & Tools
- [Eigenfaces for Recognition](https://www.researchgate.net/publication/2393986_Eigenfaces_for_Recognition) by Matthew Turk and Alex Pentland.
- [NumPy Documentation](https://numpy.org/)
- [Matplotlib Documentation](https://matplotlib.org/)

For further details and results, refer to the project report and the notebook included in this repository.
