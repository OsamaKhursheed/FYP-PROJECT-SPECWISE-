# FYP-PROJECT-SPECWISE-
SpecWise is an AI-based web app that suggests optimal PC hardware based on software needs using LLMs and real-time web scraping. It helps users, especially non-tech users, build performance-efficient and cost-effective PC setups.

# 💻 SpecWise – Intelligent PC Hardware Suggestions

**SpecWise** is an AI-powered web platform that recommends the most suitable PC hardware configurations based on your software needs. Designed especially for non-technical users, it uses Large Language Models (LLMs), machine learning, and real-time web scraping to provide performance-efficient and budget-friendly PC build suggestions.

---

## 🚀 Features

- 🧠 **AI-Powered Hardware Suggestions** via Mistral-7B LLM
- 💬 **Prompt-Based Input** (e.g., “I want to edit 4K videos in Premiere Pro”)
- 🌐 **Real-Time Web Scraping** from e-commerce websites like BestBuy
- 🛠️ **Cost & Performance Comparison** for recommended components
- 📊 **Interactive React Frontend** with seamless SPA experience
- 📂 **User History, Reviews, and Admin Panels**
- 🔍 **Fuzzy Search API** to explore hardware items
- 🧪 **White-box & Black-box Tested System**

---

## ⚙️ Tech Stack

| Layer       | Technologies                                     |
|-------------|--------------------------------------------------|
| **Frontend**| ReactJS, React Bootstrap, Axios                  |
| **Backend** | Django, Django REST Framework                    |
| **AI/ML**   | Mistral-7B (Hugging Face API), Scikit-learn      |
| **Scraping**| Selenium, BeautifulSoup                          |
| **Database**| SQLite (Django ORM)                              |
| **Others**  | Pandas, FuzzyWuzzy, ThreadPoolExecutor, Regex    |

---

## 📁 Project Structure

SpecWise/
├── frontend/ # ReactJS Frontend
├── backend/ # Django Backend
│ ├── api/ # REST APIs
│ ├── scraping/ # Web Scraping Scripts
│ ├── recommender/ # LLM Prompt System
│ └── reports/ # Report & History Management
├── media/ # Scraped JSON & Archives
├── requirements.txt # Python dependencies
└── README.md

yaml
Copy
Edit

---

## 🧠 How It Works

1. **User Input** – User provides software/task as a prompt.
2. **LLM Processing** – LLM (Mistral-7B) extracts and understands the input.
3. **Recommendation** – Suitable PC hardware is generated.
4. **Comparison** – Web scraper fetches current prices and availability.
5. **Result Display** – Recommended specs are shown to the user with links.
6. **Storage** – Logged-in users’ queries are saved for history and reports.

---

## 📦 Installation

### 1. Backend Setup (Django)
```bash
cd backend
python -m venv venv
source venv/bin/activate  # or venv\Scripts\activate
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
2. Frontend Setup (React)
bash
Copy
Edit
cd frontend
npm install
npm start
📌 API Endpoints
/api/recommend/ – Get LLM hardware recommendations

/api/scrape/ – Trigger or view scraped data

/api/fuzzy-search/ – Search products by name/type

/api/history/ – View previous queries and results (logged-in users)

/api/sync-products/ – Sync scraped products to DB

Detailed API documentation available in the /docs folder (coming soon)

🧪 Testing Summary
✅ White-box Tests
Sync Product APIs

LLM prompt processing

Recommendation pipeline

✅ Black-box Tests
Guest vs Logged-in user behavior

Mobile experience

Review submissions

🧠 Future Enhancements
Personalized recommendations based on existing hardware

Add support for multiple e-commerce platforms

Full mobile-responsive UI

Export builds to cart on vendor sites

API rate-limiting & logging dashboard

🧑‍💻 Team
Name	Email
Osama Khursheed	osamakhursheedc27@gmail.com
Shaheer Muhammad Shahbaz	shah.az0912@gmail.com
Shaheer Adil	adilshaheer09@gmail.com
Almirah Naeem	almirahnaeem74@gmail.com

Supervisor: Muhammad Timur
Institute: Usman Institute of Technology (UIT), Karachi
Batch: BSCS 2021

