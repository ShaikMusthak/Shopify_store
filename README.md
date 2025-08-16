# ChandraGenAI - Shopify Store Insights-Fetcher

A Python FastAPI app to fetch and organize brand/store insights from any Shopify-powered website, **without using the Shopify API**.

## Features

- Returns product catalog, hero products, policies, FAQs, social handles, contacts, about, important links, and more.
- Clean, modular, production-ready backend code.
- Ready for extension (competitors, MySQL, UI, etc).

## Setup

```bash
git clone https://github.com/yourusername/ChandraGenAI.git
cd ChandraGenAI
python3 -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate
pip install -r requirements.txt
uvicorn app.main:app --reload
```

Visit [http://127.0.0.1:8000/docs](http://127.0.0.1:8000/docs) for interactive API docs.

## Example Request

```json
POST /brand-insights/
{
  "website_url": "https://memy.co.in"
}
```

## Testing

```bash
pytest
```

---