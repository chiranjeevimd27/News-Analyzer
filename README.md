# News Summarization and Text-to-Speech (TTS) Application

## 📌 Project Overview
This web-based application extracts key details from multiple news articles related to a given company, performs sentiment analysis, conducts comparative analysis, and generates a text-to-speech (TTS) output in Hindi.

## 🚀 Features
- **News Extraction**: Scrapes 10+ non-JS web links for news articles using `BeautifulSoup`.
- **Summarization**: Generates concise summaries for each article.
- **Sentiment Analysis**: Categorizes news articles as `Positive`, `Negative`, or `Neutral`.
- **Comparative Analysis**: Highlights differences in news coverage across articles.
- **Text-to-Speech (TTS)**: Converts structured reports into Hindi speech.
- **User Interface**: Interactive UI built with `Streamlit` or `Gradio`.
- **API Development**: RESTful API for frontend-backend communication.
- **Deployment**: Hosted on Hugging Face Spaces.

---

## 🛠️ Tech Stack
- **Backend**: Python, FastAPI
- **Frontend**: Streamlit/Gradio
- **Web Scraping**: BeautifulSoup
- **Sentiment Analysis**: VADER/ TextBlob
- **TTS Model**: Open-source Hindi TTS engine (e.g., Vakyansh)
- **Deployment**: Hugging Face Spaces

---

## 📂 Project Structure
```
📦 NewsSummarizationTTS
├── 📂 src
│   ├── app.py             # Main application script
│   ├── api.py             # API endpoints
│   ├── utils.py           # Helper functions
│   ├── scraper.py         # News extraction logic
│   ├── sentiment.py       # Sentiment analysis module
│   ├── tts.py             # TTS conversion logic
│   ├── requirements.txt   # Dependencies
│   ├── config.py          # Configuration settings
├── README.md              # Project documentation
└── deployment
    ├── Dockerfile         # Containerization
    ├── deployment.yaml    # Kubernetes deployment config
```

---

## 🔧 Installation & Setup
### 1️⃣ Clone the Repository
```bash
git clone https://github.com/your-repo/news-summarization-tts.git
cd news-summarization-tts
```

### 2️⃣ Install Dependencies
```bash
pip install -r requirements.txt
```

### 3️⃣ Run the Application
```bash
streamlit run app.py
```

### 4️⃣ Deploy on Hugging Face Spaces
- Create a new Hugging Face Space.
- Upload the project files.
- Configure `app.py` as the main execution script.

---

## 📡 API Endpoints
| Endpoint | Method | Description |
|----------|--------|-------------|
| `/fetch-news` | `POST` | Fetch news articles for a given company |
| `/analyze` | `POST` | Perform sentiment analysis and comparative analysis |
| `/tts` | `POST` | Convert text summary to Hindi speech |

---

## 🔍 Example Usage
### Request:
```json
{
  "company": "Tesla"
}
```

### Response:
```json
{
  "Company": "Tesla",
  "Articles": [
    {
      "Title": "Tesla's New Model Breaks Sales Records",
      "Summary": "Tesla's latest EV sees record sales in Q3...",
      "Sentiment": "Positive",
      "Topics": ["Electric Vehicles", "Stock Market", "Innovation"]
    }
  ],
  "Final Sentiment Analysis": "Tesla’s latest news coverage is mostly positive.",
  "Audio": "[Play Hindi Speech]"
}
```

---

## 📄 Documentation
1. **Model Details**
   - Uses BeautifulSoup for news extraction.
   - VADER/TextBlob for sentiment analysis.
   - Open-source Hindi TTS model for speech generation.

2. **Deployment**
   - Hosted on Hugging Face Spaces.
   - Uses FastAPI for API.

3. **Limitations**
   - Requires non-JS websites for scraping.
   - May not handle real-time stock market sentiment shifts.

---

## 🎥 Submission Guidelines
✅ **GitHub Repository**: Link with structured codebase.
✅ **Hugging Face Spaces**: Hosted app link.
✅ **Video Demonstration**: Explanation of functionality.

📌 *Deadline: 1 Week*

---

## ✨ Bonus Features
- Interactive search queries over articles.
- Advanced NLP techniques for sentiment analysis.
- CI/CD pipeline integration.

---

🚀 **Happy Coding!**

