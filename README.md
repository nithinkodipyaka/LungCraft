# LungCraft: 3D Modeling and Machine Learning for Lung Cancer Diagnosis

## Overview
LungCraft is an innovative project combining 3D visualization and machine learning (ML) to enhance the diagnostic process for lung adenocarcinoma using CT scans. It features four main modules: **3D Static Reconstruction**, **Interactive 3D Visualization**, **3D Tumor Plotting**, and **Machine Learning for Classification**. The project processes diagnostic contrast-enhanced CT images and leverages quantitative imaging features and hybrid neural networks to deliver accurate, interpretable results.

---

## Project Modules

### 1. 3D Static Reconstruction
This module transforms DICOM-format CT scan slices into a cohesive 3D representation. It uses the Marching Cubes algorithm to create detailed, static 3D models of lungs. 

- **Key Features**:
  - Uniform voxel resampling to ensure consistent resolution (1mm x 1mm x 1mm).
  - Segmentation of lung structures using Hounsfield Units.
  - Static visualization of lung contours and internal structures.

- **Applications**: Provides clinicians with a clear and intuitive view of lung anatomy, enabling improved understanding of tissue density variations and abnormalities.

![Static 3D Reconstruction Example](./img/static_3d_lung.png)

---

### 2. Interactive 3D Visualization
This module enables clinicians to dynamically interact with the 3D model, exploring different angles, depths, and regions of interest.

- **Key Features**:
  - Real-time manipulation of 3D models using Plotly for interactive exploration.
  - Adjustable transparency and color schemes for better depth perception.
  - Surface rendering with Marching Cubes to highlight critical anatomical features.

- **Applications**: Enhances diagnostic precision by allowing medical professionals to examine subtle morphological complexities interactively.

![Interactive Visualization Example](./img/interactive_3d_lung.png)

---

### 3. 3D Tumor Plotting
This module overlays tumor location and size onto segmented 3D lung models, using tumor metadata provided in real-world coordinates.

- **Key Features**:
  - Mapping tumor metadata onto 3D voxel space.
  - Precise tumor localization visualized with scatter plots.
  - Integration of clinical data for enhanced prognostic assessments.

- **Applications**: Facilitates accurate surgical planning and helps clinicians assess tumor proximity to critical lung structures.

![3D Tumor Plotting Example](./img/3d_tumor_plotting.png)

---

### 4. Machine Learning for Classification
This module uses CT scan data to classify patients as diseased or healthy through advanced neural networks. The **HybridNet** architecture combines 3D and 2D convolutional layers for optimal performance.

- **Key Features**:
  - Training on preprocessed CT scans resized to uniform dimensions.
  - HybridNet achieves a training accuracy of 92% and a validation accuracy of 80%, outperforming baseline models.
  - Feature extraction focused on tumor shape complexity and intratumor density variation.

- **Applications**: Provides automated classification, aiding early diagnosis and prognosis of lung adenocarcinoma.

![Machine Learning Results Comparison](./img/ml_comparison.png)

---

## Dataset
- **Source**: [The Cancer Imaging Archive (TCIA)](https://www.cancerimagingarchive.net/)
- **Details**:
  - 4,682 contrast-enhanced CT images from 61 patients.
  - Includes clinical metadata such as survival status and tumor stage.
  - Preprocessing includes normalization, segmentation, and augmentation.

---

## Results
The project demonstrated the following:
- **Visualization**: High-resolution static and interactive 3D models enhance tumor morphology comprehension.
- **Tumor Localization**: Accurate mapping and visualization of tumor data on segmented lungs.
- **Machine Learning**: HybridNet surpassed other models like 3D CNN, ResNet, DenseNet, and UNet++ in classification accuracy and efficiency.

---

## Contributors
- **Dr. Suganya G** (VIT Chennai, Associate Professor)
- **Nithin Kodipyaka** (Researcher and Developer)

---

## License
This project is licensed under [MIT License](LICENSE).

## Contact
For further inquiries, please contact [Nithin Kodipyaka](mailto:nithinkodipyaka@example.com).

---
