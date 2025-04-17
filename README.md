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


