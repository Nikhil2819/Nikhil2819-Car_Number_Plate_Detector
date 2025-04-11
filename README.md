# 🚗 Automatic Car Number Plate Detection

<p align="center">
  <img src="images/example.png" alt="Project Screenshot" width="80%" />
</p>

---

## 📌 Overview

This project is a **Flask-based web application** that allows users to upload videos, processes them using **OpenCV** and **EasyOCR**, and detects car number plates.

The system:
- Highlights detected plates in the video
- Validates them using a regex pattern
- Outputs the **most common valid number plate** detected

---

## ✨ Features

- **📤 Upload Video**: Users can upload `.mp4`, `.avi`, or `.mov` video files.
- **🔍 Automatic Plate Detection**: Detection using contour detection and **Optical Character Recognition (OCR)** via **EasyOCR**.
- **✅ Plate Validation**: Plates are validated using a regex pattern that ensures 7 uppercase characters.

  > Regex pattern used:  
  ```python
  plate_pattern = re.compile(r'^[A-Z0-9]{7}$')
