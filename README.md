# Vitamin Deficiency Detection 🩺  
A web-based application that uses machine learning to detect potential vitamin deficiencies based on user input / symptom data and recommends possible vitamins. Built with Python (backend), web frontend (HTML/CSS), and uses a lightweight ML model for classification.  

---


## 🧠 Overview  
Vitamin Deficiency Detection is an end-to-end application that combines a pre-trained classification model (quantized) with a user-friendly web interface. Users can input their symptoms or upload relevant data, and the system predicts possible vitamin deficiencies and provides recommendations.  

This project demonstrates the integration of machine learning with a web frontend — making it accessible to non-technical users and useful for rapid prototyping of a health-related tool.

---

## 🎯 Motivation  
- To explore how machine learning models can be deployed as a lightweight, user-accessible web application.  
- To build a practical tool that helps users get a preliminary insight into possible vitamin deficiencies based on symptoms or input data.  
- To gain experience in full-stack development: data processing, ML model deployment, and frontend + backend integration.  

---

## 🛠 Tech Stack & Dependencies  

- **Python** (backend)  
- **Flask** (or similar — if you used it in `app.py`) for serving web pages and handling requests  
- **TensorFlow Lite** (or similar) — for the quantized classification model (`deficiency_classifier_quantized.tflite`)  
- **HTML / CSS / JavaScript** — for frontend user interface (`.html`, `.css`)  
- Other Python libraries (as listed in `requirements.txt`)  

---

## ✅ Features  

- User-friendly web interface for inputting symptom data / uploading dataset  
- Lightweight quantized ML model for fast inference on vitamin deficiency detection  
- Frontend + backend integration: user submits data → backend processes → returns prediction & recommendation  
- Demonstration of a full pipeline: data → model → deployment → UI  

---

## 🔍 How It Works / Methodology  

1. **Data preprocessing and feature extraction** — from user inputs or dataset to model-ready format.  
2. **Classification model (quantized)** — pre-trained on vitamin-deficiency-related data to predict deficiency classes.  
3. **Backend API (Python / Flask)** — loads the quantized model, handles incoming data, runs inference, and returns results.  
4. **Frontend UI** — HTML/CSS forms for input, displays prediction and recommended vitamins or guidance based on output.  

---

## 🚀 Getting Started / How to Run Locally  

```bash
# 1. Clone the repo  
git clone https://github.com/sarathchandra2702/Vitamin_deficiency_detection.git  

# 2. (Optional) Create and activate a virtual environment  
python3 -m venv venv  
source venv/bin/activate       # On Windows use `venv\\Scripts\\activate`  

# 3. Install dependencies  
pip install -r requirements.txt  

# 4. Run the application  
python app.py  

# 5. Open your browser and go to  
http://localhost:5000   # or whatever port is configured  
```  

Then use the web interface to input symptom data (or upload dataset) and get a vitamin deficiency prediction / recommendation.

---

## 📂 Project Structure  

```
├── app.py                               # Main backend server  
├── bnew.py / check.py                   # (Helper scripts if any)  
├── deficiency_classifier_quantized.tflite   # Quantized ML model  
├── requirements.txt                     # Python dependencies  
├── filtered_dataset.csv                 # (If any data used / sample data)  
├── html/ templates & static/ frontend files   # .html, .css for user interface  
├── demo.txt                             # Sample input / output example  
└── README.md                            # This file  
```  

---

## 📈 Results / Usage Example  

- On sample inputs provided in `demo.txt`, the model predicts vitamin deficiency (e.g., “Vitamin D deficiency”, “Vitamin B12 deficiency”, etc.) with reasonable confidence.  
- The web interface displays the prediction along with possible recommendations (vitamin types, dietary suggestions, next steps).  
- Model inference is fast due to quantization — making the app responsive and ready for lightweight deployment (e.g., as a prototype).  

> ⚠️ **Note**: This tool is **not a medical diagnostic —** it only gives a rough indication based on input symptoms. For accurate diagnosis and treatment consult a certified healthcare professional.  

---

## 🔮 Future Improvements  

- Use a **larger and more diverse dataset** for training to improve model accuracy and generalization.  
- Add **data validation and more robust feature extraction** (e.g., user demographics, diet history) for better predictions.  
- Enhance UI/UX, e.g., responsive design, better forms, user guidance, error handling.  
- Add **explainability**: show which inputs contributed most to prediction, allow users to interpret results.  
- Deploy as a **cloud/web-app** (Heroku, AWS, etc.) or create a **mobile-friendly** version.  
- Incorporate **user feedback or logging** for continuous improvement of the model.  

---

## 👨‍💻 Author  
**Sarath Chandra**  
Graduate student & Machine Learning / AI enthusiast — check out my GitHub for more projects: [@sarathchandra2702](https://github.com/sarathchandra2702)

---


