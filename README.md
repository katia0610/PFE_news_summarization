Super, j’ai consulté ton projet sur [**GitHub – PFE\_new\_summarization**](https://github.com/katia0610/PFE_new_summarization).

Voici une **suggestion complète de README.md professionnel** adaptée **exactement à ton repo actuel** pour que tu puisses la copier directement :

---

# 📰 Multimodal News Summarizer

## 🚀 Description

**Multimodal News Summarizer** est une application complète qui :

* 📄 Lit des **PDF ou images** contenant des articles de presse
* 🎧 Transcrit des **audios** (radio, podcasts)
* 🎥 Transcrit des **vidéos** (extraits de chaînes TV)
* 📝 **Corrige et nettoie** automatiquement le texte extrait
* ✂️ Génère un **résumé fidèle et synthétique** en français ou en arabe

---

## 🛠️ Stack technique

### 🔧 Backend

* **Python 3.10+**
* **FastAPI**
* **Tesseract OCR** pour l’extraction de texte sur images et PDF
* **pdf2image** pour la conversion PDF → image
* **OpenCV** pour le prétraitement d’images
* **Langdetect** pour la détection de langue
* **Groq API** :

  * **Whisper** pour la transcription audio/vidéo
  * **LLM** pour la correction et le résumé

### 🎨 Frontend

* **React JS**
  Interface utilisateur complète avec :

  * **Système d’authentification** (inscription, connexion)
  * Téléversement de fichiers (PDF, image, audio, vidéo)
  * Affichage des résumés générés automatiquement


---


## ⚙️ Installation

### 🔧 Backend

1. **Cloner le projet**

```bash
git clone https://github.com/katia0610/PFE_new_summarization.git
cd PFE_new_summarization/backend
```

2. **Installer les dépendances**

```bash
pip install -r requirements.txt
```

3. **Installer Tesseract OCR**

* **Windows :**

  * Télécharger depuis [UB Mannheim](https://github.com/UB-Mannheim/tesseract/wiki).
  * Mettre son chemin dans `constants.py` :

```python
PATH_tesseract = "C:/Program Files/Tesseract-OCR/tesseract.exe"
PATH_poppler = "C:/poppler-xx/bin"
GROQ_API_KEYS = "sk-xxxxxx"
```

* **Linux :**

```bash
sudo apt install tesseract-ocr
```

4. **Lancer FastAPI**

```bash
uvicorn main:app --reload --port 8000
```

---

### 🎨 Frontend

1. **Accéder au dossier frontend**

```bash
cd ../frontend
```

2. **Installer les dépendances**

```bash
npm install
```

3. **Lancer React JS**

```bash
npm start
```

---

## ▶️ Utilisation

* Ouvrir **[http://localhost:3000](http://localhost:3000)**
* Téléverser un **PDF, une image, une vidéo ou un audio**
* Recevoir automatiquement un **résumé clair et fidèle** de son contenu

---

## 🎯 Fonctionnalités clés

✅ Support **multimodal : PDF, image, audio, vidéo**
✅ **Détection automatique de langue** (français / arabe)
✅ **Correction orthographique et nettoyage OCR/ASR**
✅ **Résumé synthétique** avec LLM
✅ API REST backend + interface React



## 🧑‍💻 Auteur

* **Katia Bair**
  [GitHub](https://github.com/katia0610)
  
* **ET mon binome du memoire**
  

---
