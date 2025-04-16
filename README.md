# 🧭 Personalized Travel Planner with Gemini & GenAI
### A Smart Itinerary Generator Based on Location + Interests

This project is a submission for the **Gen AI Intensive Capstone by Google & Kaggle**.

It builds a fully functional **AI-powered travel assistant** that:
- Uses **semantic embeddings** to match user interests with real-world POIs
- Ranks nearby places within a **40 km radius**
- Generates a **2-day JSON itinerary** with **Gemini Pro**
- Visualizes the day-wise plan using **Folium maps and polylines**

---

## 🚀 Features

| Feature | Description |
|--------|-------------|
| 🧠 **Gemini Embeddings** | Encodes POI metadata and user interests using `embedding-001` |
| 🔍 **Vector Search** | Matches user interest with POIs using cosine similarity |
| 📦 **Structured JSON Generation** | Gemini Pro outputs itinerary in strict JSON format |
| 🗺️ **Folium Map** | Interactive map showing day-wise stops and travel routes |
| 📚 **Multi-source Data** | Museums, Restaurants, Natural Sites, and Metro Stations in Arizona |

---

## 🔧 Tech Stack

- **Python**
- **Google Generative AI (Gemini)**
- **Pandas**
- **Scikit-learn**
- **Folium**
- **Jupyter Notebook (Kaggle environment)**

---

## 📂 Dataset Sources

- [IMLS Museum Directory](https://www.kaggle.com/datasets/imls/museum-directory/data)
- Yelp Academic Dataset (subset)
- GNIS: US Geological Natural Features
- Valley Metro Rail Station Data (Phoenix)

---

## 🧠 GenAI Capabilities Used

- ✅ Embeddings
- ✅ Vector Search / Similarity Scoring
- ✅ RAG (Retrieval-Augmented Generation)
- ✅ Structured Output / JSON Mode
- ✅ Grounding using real-world data

---

## 💻 Run It

You can run this notebook locally or on [Kaggle]([https://www.kaggle.com/](https://www.kaggle.com/code/rajeshanantsawant/travel-planner-personalized-itinerary-generator)).

> Make sure to store your Gemini API key securely in environment variables or Kaggle secrets:
```python
from kaggle_secrets import UserSecretsClient
GOOGLE_API_KEY = UserSecretsClient().get_secret("GOOGLE_API_KEY")
