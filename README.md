# 🩸 Automated WBC Detection & Classification

[![Python 3.10+](https://img.shields.io/badge/python-3.10+-blue.svg)](https://www.python.org/downloads/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## Overview

This project provides an _end-to-end automated system_ for detecting and classifying White Blood Cells (WBCs) from microscopic blood smear images. It replaces the tedious manual counting process with AI, delivering a detailed diagnostic report instantly.

- _Detection_: YOLOv8 localizes all WBCs in the image.
- _Classification_: EfficientNet-B0 classifies each WBC into one of four subtypes:
  - Neutrophil
  - Lymphocyte
  - Monocyte
  - Eosinophil
- _Web Application_: A professional web interface (Django + FastAPI) allows clinicians to upload images and receive a structured report (counts, N/L ratio, medical interpretation).

## 🖥️ Web Application - User Interface

The web application allows doctors to upload a microscopic image and instantly obtain a comprehensive analysis report.

### 📤 Step 1: Image Upload

The user selects an image (JPG/PNG format) via the simple interface.

![Upload Interface](results/example.jpeg)

### 📊 Step 2: Analysis Result

The image is automatically analyzed by the AI. White blood cells are outlined in different colors according to their type (Monocytes, Lymphocytes, etc.). A detailed report is displayed with:

- Total WBC count
- Count by type (Neutrophils, Monocytes, Lymphocytes, Eosinophils)
- Neutrophil/Lymphocyte (N/L) ratio
- Automatic medical interpretation

![Analysis Result](results/result.jpeg)
