# 🧠 Financial Intelligence Agent  

The **Financial Intelligence Agent** is an AI-powered assistant for **market analysis, financial research, and credit risk assessment**.  
It integrates multiple data sources (Yahoo Finance, DuckDuckGo, news scrapers) with LLM reasoning to provide actionable financial intelligence in real time.  

---

## ✨ Features  

- 🔎 **Intent Classification** – Understands user queries and routes them to the right workflow:
  - **Market Analysis** → Stock prices, fundamentals, ratios, analyst recommendations.  
  - **Research** → Investigates news, trends, implications, and industry outlook.  
  - **Credit Score** → Evaluates risk factors, financial health, and assigns a creditworthiness score.  

- 📊 **Structured Reports** – Generates executive summaries, tables for financial data, and interprets results clearly.  
- 🌐 **Multi-source Research** – Combines **Yahoo Finance**, **DuckDuckGo**, and **NewsPaper4k** for reliable insights.  
- ⚡ **LLM-powered Reasoning** – Backed by **Groq’s LLaMA-3 70B** model for advanced financial understanding.  

---

## 🛠️ Tech Stack  

- **Python 3.10+**  
- [agno](https://pypi.org/project/agno/) → Agent orchestration  
- **Groq API (LLaMA-3 70B)** → LLM inference  
- **YFinanceTools** → Stock data, fundamentals, analyst reports  
- **DuckDuckGoTools** → Web search integration  
- **Newspaper4kTools** → News & article extraction  
- **dotenv** → Secure API key management  
- **certifi** → SSL certificate validation  

---

## 📂 Applications  

- 📈 **Investors & Analysts** → Real-time market insights and stock health evaluation  
- 📰 **Researchers & Journalists** → Industry impact studies and trend analysis  
- 🏦 **Banks & Lenders** → Automated **credit risk scoring** and financial health reports  
- 🎓 **Education** → Training tool for finance & business analytics  

---

## ⚙️ Setup & Installation  

### 1. Clone the repository  
```bash
git clone https://github.com/pvsaravanan/credtech.git
cd credtech
```

### 2. Create & activate a virtual environment  
```bash
python -m venv venv
source venv/bin/activate   # Mac/Linux
venv\Scriptsctivate      # Windows
```

### 3. Install dependencies  
```bash
pip install -r requirements.txt
```

### 4. Configure Environment Variables  
Create a `.env` file in the project root:  
```ini
GROQ_API_KEY=your_groq_api_key
PHI_API_KEY=your_phi_api_key
```

### 5. Run the agent  
```bash
python main.py
```

---

## 📊 Example Usage  

```python
user_query = "Evaluate Meta creditworthiness and provide a risk assessment"
intent = classify_intent(user_query)
print(f"Detected Intent: {intent}")

financial_intelligence_agent.print_response(user_query, stream=True)
```

**Output (sample)**  
```
Detected Intent: credit_score

Executive Summary:
Meta shows strong fundamentals with manageable debt ratios. Risk is moderate to low.  

Creditworthiness Score: 8.5/10  
Interpretation: Investment Grade – Low risk of default.  

[Table with key financial ratios]
```

---

## 🚀 Roadmap  

- [ ] Add **FREDTools** for macroeconomic indicators  
- [ ] Deploy as a **REST API / FastAPI service**  
- [ ] Build a **frontend dashboard** (Streamlit or Next.js)  
- [ ] Add **memory & conversation history** for richer interactions  

---

## 📜 License  

MIT License © 2025  
