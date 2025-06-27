# 📰 Multimodal News Summarizer

## 🚀 Description

**Multimodal News Summarizer** is a complete application that:

* 📄 Reads **PDFs or images** containing news articles
* 🎧 Transcribes **audio files** (radio, podcasts)
* 🎥 Transcribes **videos** (TV extracts, news reports)
* 📝 **Cleans and corrects** the extracted text automatically
* ✂️ Generates a **faithful and concise summary** in French or Arabic

---

## 🛠️ Tech Stack

### 🔧 Backend

* **Python 3.10+**
* **FastAPI**
* **Tesseract OCR** for text extraction from images and PDFs
* **pdf2image** for PDF → image conversion
* **OpenCV** for image preprocessing
* **Langdetect** for language detection
* **Groq API**:

  * **Whisper** for audio/video transcription
  * **LLM** for correction and summarization

### 🎨 Frontend

* **React JS**
  A complete user interface with:

  * **Authentication system** (sign up, login)
  * File upload (PDF, image, audio, video)
  * Display of the automatically generated summaries

---

## ⚙️ Installation

### 🔧 Backend

1. **Clone the project**

```bash
git clone https://github.com/katia0610/PFE_new_summarization.git
cd PFE_new_summarization/backend
```

2. **Install dependencies**

```bash
pip install -r requirements.txt
```

3. **Install Tesseract OCR**

* **Windows:**

  * Download from [UB Mannheim](https://github.com/UB-Mannheim/tesseract/wiki).
  * Set its path in `constants.py`:

```python
PATH_tesseract = "C:/Program Files/Tesseract-OCR/tesseract.exe"
PATH_poppler = "C:/poppler-xx/bin"
GROQ_API_KEYS = "sk-xxxxxx"
```

* **Linux:**

```bash
sudo apt install tesseract-ocr
```

4. **Run FastAPI**

```bash
uvicorn main:app --reload --port 8000
```

---

### 🎨 Frontend

1. **Navigate to the frontend folder**

```bash
cd ../frontend
```

2. **Install dependencies**

```bash
npm install
```

3. **Run React JS**

```bash
npm start
```

---

## ▶️ Usage

* Open **[http://localhost:3000](http://localhost:3000)**
* Upload a **PDF, image, video, or audio file**
* Automatically receive a **clear and faithful summary** of its content

---

## 🎯 Key Features

✅ **Multimodal support:** PDF, image, audio, video
✅ **Automatic language detection** (French / Arabic)
✅ **OCR/ASR text cleaning and correction**
✅ **Concise summarization** with LLM
✅ REST API backend + React interface

---

## 🧑‍💻 Authors

* **Katia Bair**
  [GitHub](https://github.com/katia0610)

* **And my thesis teammate**

