### 🧠 MedalyZe: AI-Base-Disease-and-Medicine-Recommender

MedalyZe is a Flask-based AI web app that predicts diseases from user-entered symptoms and recommends treatment, medicines, precautions, and diet. It uses NLP and machine learning techniques to provide intelligent analysis from both short phrases and detailed symptom descriptions.

---

##  Project Structure

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

##  Installation & Setup

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

## 📞 Contact
Developed by
[Github](https://github.com/aniket-next). <br>
[LinkedIn](https://www.linkedin.com/aniiiket-singh)<br>
[Email] (anikxtpro@gmail.com)<br>
[Instagram](https://www.instagram.com/aniiiket.siiingh)<br>
[X/twitter](https://www.x.com/Aniiiketsiingh)

For queries, open an issue or contact via GitHub or other social media.

---

Happy diagnosing with 💡 MedalyZe!
