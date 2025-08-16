# Shaik Musthak - Shopify Store Insights-Fetcher

A Python **FastAPI** application to fetch and organize brand/store insights from any **Shopify-powered website**, **without relying on the Shopify API**.  
This project is designed to showcase **clean backend development**, **data scraping/parsing**, and **REST API design**.

---

## 🚀 Features

- Extracts product catalog, hero products, policies, FAQs, social handles, contacts, about info, and important links.  
- Built with **FastAPI** → automatic docs (`Swagger` & `ReDoc`).  
- **Clean, modular, production-ready** backend code.  
- Ready for **extension**:
  - Competitor analysis
  - Database integration (MySQL / PostgreSQL / MongoDB)
  - Frontend UI (React / Next.js)
  - Cloud deployment (AWS / GCP / Azure)

---

## 🛠️ Tech Stack

- **Python 3.8+**
- **FastAPI** (for API backend)
- **BeautifulSoup4 / Requests** (for scraping Shopify stores)
- **Pytest** (for testing)
- **Uvicorn** (for ASGI server)

---

## 📂 Project Structure

Musthak_shopify/
│── app/
│ ├── api/ # API routes
│ │ └── endpoints.py
│ ├── core/ # Core scraping logic
│ │ └── scraping.py
│ ├── models/ # Pydantic models
│ │ └── brand.py
│ ├── utils/ # Utility functions
│ │ └── helpers.py
│ └── main.py # FastAPI app entry point
│
│── tests/
│ └── test_api.py # Unit tests
│
│── requirements.txt # Dependencies
│── README.md # Documentation

---

## ⚙️ Setup

```bash
# Clone repository
git clone https://github.com/ShaikMusthak/Shopify_store.git
cd Shopify_store

# Create virtual environment
python3 -m venv venv
source venv/bin/activate   # Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Run server
uvicorn app.main:app --reload

---

## 📡 Example Request
POST /brand-insights/
{
  "website_url": "https://memy.co.in"
}
---
## 👤 Author

Shaik Musthak
