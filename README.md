# Auto Barcode Generating as Per Plan AI

This project is an AI-powered web tool that automates the generation of barcodes from VIN (Vehicle Identification Number), performs VIN decoding, and extracts VINs from images using OCR. It supports both Indian and US vehicles.

---

## 🚀 Features

- 📦 VIN to Barcode/QR Code Generator
- 🔍 VIN Decoding (US via NHTSA API, Indian via pattern logic)
- 🧠 OCR VIN Recognition from Images
- 📄 Plan File Upload (Excel/CSV)
- 💻 Web Interface (Flask-based)
- 📤 Batch Barcode Export (ZIP or PDF)
- 📱 Mobile-Friendly UI

---

## 🛠️ Tech Stack

- Python (Flask, Pandas, Requests)
- Barcode Tools: `python-barcode`, `qrcode`
- OCR: `EasyOCR`, `OpenCV`
- VIN Decoding API: [NHTSA VIN API](https://vpic.nhtsa.dot.gov/api/)
- Frontend: HTML, Bootstrap

---

## 📂 Folder Structure

auto-barcode-ai/ ├── app.py # Flask server ├── static/ │ └── barcodes/ # Generated barcode images ├── templates/ │ └── index.html # Web UI ├── utils/ │ ├── vin_decoder.py # VIN decoding logic │ ├── barcode_generator.py │ └── ocr_reader.py ├── uploads/ # Plan & image uploads ├── requirements.txt └── README.md

---




---

## 🔄 Workflow

1. Upload your **VINs plan file (CSV/XLSX)** or **enter VIN manually**.
2. System generates **1D/QR barcodes** and displays them.
3. Option to **download barcodes as PDF or ZIP**.
4. Upload **image with VIN** → system uses **OCR** to extract.
5. System **decodes VIN** (Indian or US) and displays details.

---

## 🔧 Setup Instructions

bash
# Clone the repo
git clone https://github.com/your-username/auto-barcode-ai.git
cd auto-barcode-ai

# Create virtual environment
python -m venv venv
source venv/bin/activate  # or venv\Scripts\activate on Windows

# Install dependencies
pip install -r requirements.txt

# Run the Flask app
python app.py
----Open http://localhost:5000 in your browser.----




----




📸 Sample VIN Image

[ Upload an image of VIN label ]
→ System extracts and shows: MH12BC12345678900
→ Decoded: Model, Make, Year, Engine, etc.

-----








