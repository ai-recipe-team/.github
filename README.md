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
| Frontend             | HTML + Flask                       |
| Deployment           | (Optional: Render / Google Colab)  |

---

## 📁 Project Structure

ai-recipe-suggester/
├── app.py # Main Flask app
├── yolo_detect.py # Image detection (YOLOv8)
├── NLP_code.py # Preprocessing and food filtering
├── llm_module.py # Gemini-based recipe generation
├── templates/
│ └── index.html # Frontend form
├── uploads/ # Uploaded images folder
├── .gitignore
├── requirements.txt
├── CONTRIBUTING.md
└── README.md # You're here!



---

## 👥 Team Contributors

| Name               | Role                          |
|--------------------|-------------------------------|
| Gourika Khandelwal | Frontend Design & Integration |
| Sachita Singla     | YOLOv8 Detection Module       |
| Lipi Goel          | LLM-based Recipe Generator    |
| Minakshi Kaushik   | NLP Filtering & App Logic     |

> 🤝 A collaborative team project built with shared ownership and equal contribution.

---

## 🛠️ Getting Started

```bash
# Clone the repo
git clone https://github.com/YOUR-USERNAME/ai-recipe-suggester.git
cd ai-recipe-suggester

# (Optional) Create and activate a virtual environment
python -m venv venv
source venv/bin/activate  # For Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Run the app
python app.py
🔐 API Key Setup (for Gemini API)
To use Gemini for recipe generation, create a .env file in the project root and add your API key like this:

ini
Copy code
GEMINI_API_KEY=your_gemini_api_key_here
Then, in your Python code, access the key using:

python
Copy code
import os
api_key = os.getenv("GEMINI_API_KEY")
✅ Make sure your .env file is listed in .gitignore to keep it private.
🔑 You can get your Gemini API key from: https://makersuite.google.com/app/apikey

🧑‍🍳 Built with curiosity, teamwork, and a love for food & AI!
