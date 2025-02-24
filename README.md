# A-Pharmacist-Diagnostic-Assistant
This project utilizes an AI-powered Pharmacist’s Assistant through the application of OCR (Tesseract) to recognize text on handwritten prescriptions and match them against a specified medicine database. This makes medicine identification efficient and enables the automatic generation of pharmacy orders. The Diagnostic Assistant also helps medical professionals analyze medical scans, patient reports, and symptoms to diagnose diseases.

Features : - 
1. Handwritten Prescription Processing: Uses Tesseract OCR to extract text from prescription images, simplifying medicine identification.
2. Order Matching & Generation: Cross-references extracted text with a standardized drug database to generate pharmacy orders automatically.
3. Medical Image Processing: Utilizes deep learning (CNNs) to analyze medical images.
4. Symptom-Based Diagnosis: Uses NLP/ML to suggest possible diseases based on symptoms.
5. Preprocessing for Improved OCR: Applies grayscale conversion, thresholding, and noise reduction to enhance text extraction accuracy.
6. Error Reduction and Accuracy Enhancement: Improves text recognition through adaptive thresholding and denoising techniques.
7. Scalability: Designed to integrate seamlessly with hospital and pharmacy databases.

Installation & Setup
Prerequisites
Ensure the following dependencies are installed:
Python 3.x
OpenCV
Tesseract OCR
NumPy
Matplotlib
pytesseract
Flask (optional, for API integration)
TensorFlow/Keras or PyTorch (for deep learning-based medical image analysis)

Install Dependencies
pip install numpy opencv-python pytesseract matplotlib flask tensorflow torch torchvision

Install Tesseract OCR
On Linux: - 
sudo apt-get install tesseract-ocr.

On Windows: -
Download and install Tesseract from Tesseract OCR GitHub.

Set Up the Project
Clone this repository and navigate to the project directory:

git clone https://github.com/your-repo/pharmacist-assistant.git
cd pharmacist-assistant

Running the Code
Extract Text from a Handwritten Prescription
1. Place the prescription image in the project directory (e.g., prescription.jpg).
2. Run the script: - python main.py
3. The extracted text will be displayed in the console, along with the processed image.
4. The system will match the extracted text with recognized medicines and generate an order.

Medical Image Processing
1. Store medical images in the designated directory.
2. Modify image_analysis.py to specify the correct image path.
3. The system will analyze the image and provide diagnostic results.

Update Image Path
Modify the image_path variable in main.py or image_analysis.py if necessary.

Future Enhancements
1. Advanced medicine database integration for more accurate order generation.
2. Machine learning-powered handwriting recognition for improved OCR accuracy.
3. Deep learning-based medical image classification.
4. A web-based interface for real-time prescription processing and diagnostics.
