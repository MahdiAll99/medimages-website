---
title: "🧠 Radiomics in medical imaging: A brief introduction"
summary: A concise introduction to radiomics and a showcase of the typical workflow for radiomics analysis.
date: 2023-03-05

# Featured image
# Place an image named `featured.jpg/png` in this page's folder and customize its options here.
image:
  caption: 'Image credit: [**Review on Radiomics for Brain Tumors**](https://med.stanford.edu/gevaertlab/ReviewRadiomicsBrain.html?tab=proxy)'

authors:
  - Mahdi Loutfi

tags:
  - Radiomics
  - Medical Imaging
  - Cancer
  - Python
  - Machine Learning
---

Welcome 👋

The aim of the present blog is to give a brief introduction to radiomics and present a typical workflow of radiomics analysis.

## Overview

1. Radiomics is a technique for the quantitative description of multi-modal medical images.
2. An overview on radiomics analysis typical workflow.
3. Useful links and and open-source resources that can help enhance your understanding of radiomics.

[//]: # ([![The template is mobile first with a responsive design to ensure that your site looks stunning on every device.]&#40;https://raw.githubusercontent.com/wowchemy/wowchemy-hugo-modules/main/starters/academic/preview.png&#41;]&#40;https://hugoblox.com&#41;)

### AI in medecine

In recent decades, the medical industry has experienced a consistent rise in the digitization of clinical data. Additionally, the methods of artificial intelligence (AI) have become not powerful and accessible enough to put the focus on identifying the most relevant data and the information most likely to be helpful to solve a given issue. Consequently, there has been a substantial increase in AI applications in healthcare, with the aim of simplifying repetitive tasks clinicians encounter in their daily workflows and promoting the advancement of personalized medicine.

Machine learning (ML) is a subset of AI with promising tools that can assist the medical field in tasks like classification, segmentation, and more. Deep learning (DL) is a specific branch of ML that involves using multiple layers of neural networks to detect and/or extract features in imagery. Most AI-based medical field tasks are conducted using DL algorithms. However, in the realm of ML-based classification of medical imaging data, radiomics is a well-established competitor to DL. When compared to DL, radiomics features are highly explainable since they are based on mathematical definitions. As a result, radiomics is highly capable of handling massive amounts of data in the medical field, with the goal of delivering precision medicine.

## What is radiomics?

Radiomics refers to the high-throughput quantitative image analysis which aims at extracting a large number of features characterizing a region of interest in the medical image. Radiomics analysis can be performed on medical images from different modalities, e.g., from from magnetic resonance imaging (MRI), computed tomography (CT), and positron-emission-tomography (PET). This approach enhances the existing data available to clinicians by quantifying the spatial distribution of signal intensities, voxels interrelationships and textural information.

### Radiomics typical workflow

The figure below demonstrates the necessary stages in a typical radiomics pipeline, emphasizing the crucial aspects of the radiomics analysis procedure.

![Radiomics typical workflow](https://miro.medium.com/v2/resize:fit:720/format:webp/1*N3OwjGfL6z0TasMeK0s6xg.png)

- **Segmentation**: For every radiomics analysis, the region of interest (ROI) definition is crucial for the extraction of information from medical images. The images segmentation might be done manually by en expert or automatically using a deep learning model, such as [MONAI](https://monai.io/)’s model Swin UNETR.

![Segmentation](https://production-media.paperswithcode.com/thumbnails/task/1acce291-f809-41b2-b665-8ce57b31efb8.jpg)

- **Image processing**: Image processing comes after the segmentation step and before the feature extraction step. It aims to standardize images, from which radiomic features will be extracted, in terms of pixel spacing, gray-level intensities, histogram bins, etc. The main processing steps are: Interpolation, re-segmentation, ROI extraction and intensity discretization. Note that the image processing steps leading to features computation can be carried out in various ways, in terms of processing parameters. A separate blog post will be written specifically for the image processing steps.

![Image processing](https://miro.medium.com/v2/resize:fit:720/format:webp/1*Md-OJnazNB7bXKNXa_LZog.png)

- **Features extraction**: Following image segmentation and processing, features can be extracted from the image. Feature extraction is the final processing step where feature descriptors are utilized to quantify characteristics of the grey levels within the ROI. The set of features can be classified into various families, including intensity-based statistical features, intensity histogram-based features, intensity-volume histogram-based features, morphological features, local intensity features, and texture matrix-based features. Each family has the potential to reveal tumoral patterns, size, shape, and textural characteristics that may not be discernible to the naked eye. Additionally, features can be computed on the base image, as well as from filtered images.

![Features extraction](https://miro.medium.com/v2/resize:fit:720/format:webp/1*Lm7_aUPWdE0YBuqPGh9R-Q.png)

## Useful links for radiomics

- PyRadiomics package: https://github.com/AIM-Harvard/pyradiomics. 
- MEDimage package: https://github.com/MahdiAll99/MEDimage.
- Radiomics in medical imaging — “how-to” guide and critical reflection: https://doi.org/10.1186/s13244-020-00887-2.
- IBSI: https://theibsi.github.io/.

[**Image references can be found here.**](https://medium.com/@mahdiall99/radiomics-in-medical-imaging-a-brief-introduction-3208863aae87)
