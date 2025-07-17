# 🧠 MedalyZe: AI-Powered Disease and Medicine Recommender

MedalyZe is a Flask-based AI web app that predicts diseases from user-entered symptoms and recommends treatment, medicines, precautions, and diet. It uses NLP and machine learning techniques to provide intelligent analysis from both short phrases and detailed symptom descriptions.

---

## 📁 Project Structure

```
medalyze/
├── templates/              # HTML files (index.html, about.html, contact.html)
├── static/                 # CSS, JS, and images
│   ├── styles.css
│   └── script.js
├── data/
│   ├── decease.csv         # Disease and symptoms dataset
│   └── med.csv             # Medical info (medicines, precautions, diet)
├── models/                 # Trained ML models (after training)
├── logs/                   # Log files (auto-created)
├── main_app.py            # Main Flask application
├── train_disease.py       # Script to train disease prediction model
├── config.py              # Configuration file (paths, settings)
├── requirements.txt       # Python dependencies
├── .env.example           # Sample environment config
└── README.md              # Project guide (this file)
```

---

## ⚙️ Installation & Setup

### 1. Clone the Repository
```bash
git clone https://github.com/aniket-next/MedalyZe_AI_base_disease_and_medicine_recommendation.git
cd MedalyZe_AI_base_disease_and_medicine_recommendation
```

### 2. Create Virtual Environment (Python 3.9)
```bash
conda create -p ./venv python=3.9 -y
conda activate ./venv
```

> ✅ Make sure you see `(venv)` in your terminal.

### 3. Install Dependencies
```bash
pip install -r requirements.txt
```

### 4. Configure Environment Variables
Copy the example file and fill in real values if needed:
```bash
cp .env.example .env
```
You can set your `SECRET_KEY` and toggle `FLASK_DEBUG` in `.env`.

---

## 🧠 Training the Model
If you haven't trained your ML model yet:
```bash
python train_disease.py
```
> This will generate `disease_model.pkl` and `disease_vectorizer.pkl` inside the `models/` directory.

---

## 🚀 Run the App
```bash
python main_app.py
```
Then visit: [http://127.0.0.1:5000](http://127.0.0.1:5000)

---

## 📌 Notes
- ❌ **Do NOT upload `.env` or `models/` to GitHub.** They should be in `.gitignore`.
- ✅ You SHOULD upload `.env.example` so others know what to configure.
- ✅ You SHOULD train the model once and keep the generated `.pkl` files locally.

---

## ✅ GitHub Setup Checklist
- [x] `.gitignore` includes `.env`, `venv/`, `*.pkl`, `__pycache__/`
- [x] `.env.example` is included
- [x] Code is tested with Python 3.9
- [x] README has install/run instructions

---

## 🧪 Run Tests (Optional)
If you want to run full unit/integration tests:
```bash
python test_disease_predictor.py
```

---

## 📞 Contact
Developed by [aniket-next](https://github.com/aniket-next). For queries, open an issue or contact via GitHub.

---

Happy diagnosing with 💡 MedalyZe!
