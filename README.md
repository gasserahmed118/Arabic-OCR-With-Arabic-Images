📝 OCR Comparison: Pytesseract vs EasyOCR A project comparing the performance of two popular OCR engines on English text images.

📌 Overview This project performs Optical Character Recognition (OCR) using two different libraries: Pytesseract – a Python wrapper for Google’s Tesseract OCR engine EasyOCR – a modern deep learning–based OCR library

The goal is to evaluate how both tools perform in recognizing Arabic text from images, observe differences in accuracy, speed, and robustness, and visualize the extracted text.

Pytesseract is a Python wrapper for Google’s Tesseract OCR engine, one of the most widely used OCR systems. It is based on traditional OCR algorithms (LSTM-based recognition starting from v4). 
⭐ Key Features : Open-source and free , Works best with clean, high-contrast images , Supports many languages , Very fast on CPU , Does not require a GPU , Traditional OCR, not deep learning

⚙️ How Pytesseract Works :
Load the image and convert to RGB
Preprocess if needed (resize, threshold, denoise)
Call pytesseract.image_to_string()
Split results into lines
Display text for each image

EasyOCR is a deep-learning based OCR library uses as a deep learning detection and recognition model ⭐
Key Features : Very high accuracy for many languages , Can detect text in complex real-world scenarios , Supports 80+ languages , Provides bounding boxes + confidence scores , Uses PyTorch backend , Slower than Tesseract but more accurate

⚙️ How EasyOCR Works
Load the OCR reader
Pass an image to readtext()
It returns: bounding box recognized text confidence score
Optionally visualize the image

Visualization : The details of the image is showen as each model detects them
