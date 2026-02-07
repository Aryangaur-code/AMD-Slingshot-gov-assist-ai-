# AMD-Slingshot-gov-assist-ai-
A voice-first, explainable AI system for inclusive access to government welfare schemes in India, designed for edge–cloud deployment on AMD platforms


# 🏛️ GovAssist AI — Powered for AMD Slingshot

**A voice-first, explainable AI system for inclusive access to government welfare schemes in India, designed for edge–cloud deployment on AMD platforms.**

> Built for the **AMD Slingshot Competition 2025** by **CYBERNETICS CREW BIT**

---

## 🌍 Problem Statement  

Millions of Indian citizens—particularly in rural and low-literacy communities—struggle to access government welfare schemes because of:

- Low digital literacy  
- Complex and opaque eligibility rules  
- Confusing document requirements  
- Language barriers  
- Dependence on exploitative middlemen  
- High application rejection rates  
- Poor accessibility of text-heavy portals  

This creates a severe last-mile governance gap where the most vulnerable citizens are excluded from their rightful benefits.

---

## 💡 Our Solution — GovAssist AI  

**GovAssist AI** is an **AMD-optimized, edge–cloud AI assistant** that enables citizens to:

- Speak naturally in their local language  
- Discover **personally eligible schemes**  
- Understand **why they qualify (Explainable AI)**  
- Receive a verified **document checklist**  
- Fill forms **using voice**  
- Reduce errors through **AI reconfirmation**  
- Navigate directly to official government portals  
- Access simple, rights-based guidance in regional languages  

### Motto  
> **“Right Scheme. Right Person. Right Documents.”**

---

## ✨ Key Features  

- 🎙️ **Voice-first rural access** using Bhashini APIs  
- 🧠 **Hybrid Rule-Based + AI Eligibility Engine**  
- 🔍 **Explainable AI (“Why Eligible?”)**  
- 📄 **Automatic document checklist generation**  
- 📝 **Voice-based form filling with validation**  
- ✅ **Reconfirmation loop to prevent errors**  
- 🔗 **Direct redirection to official portals**  
- ⚖️ **Constitution-backed knowledge layer**  
- 🔐 **Privacy-first design with minimal data collection**  
- ⚡ **AMD Edge-accelerated pre-processing for low latency**

---

## 🖥️ AMD Integration & Innovation

### How GovAssist AI uses AMD

| Layer                         | AMD Contribution                                 |
|-------------------------------|--------------------------------------------------|
| Edge Processing (CSC Centers) | AMD CPUs for low-latency speech processing       |
| AI Inference Acceleration     | AMD GPUs for LLM reasoning & multilingual tasks  |
| Document Processing (OCR)     | Faster image pre-processing before AWS Textract  |
| Rural Deployment              | Energy-efficient, cost-effective edge nodes      |
| Hybrid AI                     | Seamless edge–cloud workload distribution        |

### Why this matters for AMD
- Real-world **public-sector AI at scale**  
- Demonstrates **edge + cloud hybrid AI**  
- Optimized for **low-bandwidth rural environments**  
- Showcases **energy-efficient, inclusive computing**

---

## ☁️ System Architecture (Edge–Cloud Hybrid)

### Edge Layer (AMD-powered)
- Local speech processing (STT/TTS)  
- Fast pre-processing of documents  
- Reduced cloud dependency  
- Lower latency for rural users  

### Cloud Layer (AWS)
- **Bhashini** — Speech & translation  
- **AWS Bedrock** — Explainability & reasoning  
- **FastAPI** — Backend services  
- **AWS Textract** — OCR validation  
- **PostgreSQL / DynamoDB** — Data storage  
- **AWS S3** — Secure document storage  
- **CloudWatch** — Monitoring & analytics  

---

## 🔄 System Workflow  

1. User speaks in local language  
2. Edge node (AMD) processes voice  
3. Bhashini converts speech to text  
4. AI extracts citizen profile  
5. Eligibility engine matches schemes  
6. AWS Bedrock explains eligibility  
7. System returns document checklist  
8. User fills forms via voice  
9. AI reconfirms details  
10. Redirect to official portal  

---

## 📊 Dataset Used  

We use the publicly available dataset:

**Indian Government Schemes Dataset (Kaggle)**  
https://www.kaggle.com/datasets/nitishabharathi/indian-government-schemes  

This dataset is enriched with:

- Eligibility logic  
- Document mappings  
- Official form references  
- Portal links  
- State-wise variations  

---

## 🛠️ Tech Stack  

- **Frontend:** React / Gradio (MVP)  
- **Backend:** Python FastAPI  
- **AI:** AWS Bedrock  
- **OCR:** AWS Textract  
- **Storage:** AWS S3  
- **Database:** DynamoDB / PostgreSQL  
- **Speech:** Bhashini APIs  
- **Edge Compute:** AMD CPU/GPU nodes  

---

## 🎯 Social Impact  

GovAssist AI aims to:

- Reduce application rejection rates  
- Eliminate dependence on middlemen  
- Increase rural digital inclusion  
- Improve welfare scheme uptake  
- Save citizens’ time and money  
- Strengthen transparent governance  

---

## 🧑‍🤝‍🧑 Team  

**Cybernetics Crew BIT**  
Birla Institute of Technology, Mesra — Jaipur Campus  

**Team Lead:** Aryan Gaur  

---

## 🚀 Future Enhancements  

- Real-time grievance submission  
- NGO/CSC admin dashboard  
- Aadhaar-based verification  
- Multi-state scheme expansion  
- Offline-first mode for remote villages  
- WhatsApp & IVR integration  

---

## 📜 License  

MIT License — Open for education, research, and social innovation.

---

## 📞 Contact  

📧 Email: aryangaur76731@gmail.com 
🔗 GitHub: https://github.com/your-username/govassist-ai  
🌐 LinkedIn: https://linkedin.com/in/your-profile  
