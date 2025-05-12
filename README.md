# 🚘 Vehicle Number Plate Detection using OCR & OpenCV

This project demonstrates automatic vehicle number plate detection using **Python**, **OpenCV**, and **Tesseract OCR**. The system processes an uploaded image, identifies the number plate region, and extracts text from it using Optical Character Recognition (OCR).

---

## 📌 Features

- Upload an image containing a vehicle.
- Automatically detects and extracts the number plate region.
- Applies OCR to recognize and read the text on the number plate.
- Preprocessing techniques to improve detection accuracy.

---

## 🛠️ Technologies Used

- Python 3
- OpenCV
- NumPy
- Tesseract OCR
- Google Colab (for execution)

---

## 🚀 How to Run

1. Open the notebook in Google Colab.
2. Install the required dependencies:
   ```bash
   !apt-get install -y tesseract-ocr
   !pip install pytesseract opencv-python
   ```
3. Upload an image of a vehicle when prompted.
4. The program will:
   - Preprocess the image.
   - Detect the number plate region.
   - Use Tesseract OCR to extract and display the plate number.

---

## 🧠 Code Breakdown

- **preprocess_image(image):** Converts to grayscale, filters noise, and applies edge detection.
- **find_plate_contour(edged):** Locates the contour of the number plate using polygon approximation.
- **extract_plate(image, contour):** Masks and crops the number plate region for OCR.

---

## 📷 Example (Optional)

> You can add before/after screenshots of the detection output here.

---

## 📚 Future Enhancements

- Train with custom datasets for Indian number plate formats.
- Add real-time video feed processing.
- Deploy as a web application using Flask or Streamlit.

---
