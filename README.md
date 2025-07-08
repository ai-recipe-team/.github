# 🧠 AI-Powered Recipe Suggester 🍽️

Turn your fridge photos into delicious meals!  
This smart web app uses **YOLO object detection**, **NLP filtering**, and **LLM-based recipe generation** to suggest creative recipes using only the ingredients you already have.

---

## 🚀 What It Does

📸 Upload an image of your fridge or kitchen  
🧠 Detect ingredients using YOLOv8  
🧹 Filter non-food items with NLP + WordNet  
🧾 Generate creative recipes using Gemini-based LLM  
🍽️ Cook something awesome — instantly!

---

## 💡 Tech Stack

| Feature              | Tech Used                         |
|----------------------|------------------------------------|
| Ingredient Detection | YOLOv8 (Ultralytics)               |
| Filtering            | Python NLP + WordNet               |
| Recipe Generation    | Gemini LLM (Google)                |
| Frontend             | Streamlit                          |
| Deployment           | Hugging Face                       |

---

## 📁 Project Structure

recipe_oracle/
│
├── script.py # Main Streamlit app (UI + logic)
├── llm_module.py # Handles interaction with Gemini API (dish suggestions, recipe steps)
├── yolo_detect.py # Detects ingredients from uploaded image using YOLO
├── NLP_code.py # Cleans & filters detected objects (removes non-ingredients)
│
├── secrets.env # 🔒 Gemini API Key (Keep it secret, don't upload)
├── requirements.txt # Python dependencies
├── README.md # Project documentation
├── team.txt # Contributors list
│
├── background.png # UI background image
├── .gitignore # Files to ignore when pushing to GitHub
│
├── uploads/ # Folder to temporarily store uploaded image
└── pycache/ # Python cache (ignored)


---

## 👥 Team Contributors

| Name               | Role                          |
|--------------------|-------------------------------|
| Gourika Khandelwal | Frontend Design               |
| Sachita Singla     | YOLOv8 Detection Module       |
| Lipi Goel          | LLM-based Recipe Generator    |
| Minakshi Kaushik   | NLP & Integration             |

> 🤝 A collaborative team project built with shared ownership and equal contribution.

---

## 🛠️ Getting Started
```bash
# 🍽️ Clone the repository
git clone https://github.com/ai-recipe-team/recipe-oracle.git
cd recipe-oracle

# 🧪 (Optional but recommended) Create and activate a virtual environment
python -m venv venv
# Activate the environment
# For Windows:
venv\Scripts\activate
# For Mac/Linux:
source venv/bin/activate

# 📦 Install required dependencies
pip install -r requirements.txt

# ▶️ Run the Streamlit app
streamlit run script.py
```

🔐 API Key Setup (for Gemini API)
```ini
To use Gemini for recipe generation, create a secrets.env file in the project root and add:
GEMINI_API_KEY=your_gemini_api_key_here
```

In Python code (already handled in llm_module.py), the key is loaded using:

```python
from dotenv import load_dotenv
import os

load_dotenv("secrets.env")
api_key = os.getenv("GEMINI_API_KEY")
```
✅ Make sure secrets.env is listed in your .gitignore so it doesn’t get pushed to GitHub.

🔑 Get Your Gemini API Key From:
https://makersuite.google.com/app/apikey


🧑‍🍳 Built with curiosity, teamwork, and a love for food & AI!
