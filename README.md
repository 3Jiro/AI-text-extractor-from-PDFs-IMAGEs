# 📝 Multi-Format OCR & Document Transformer (Telegram)
### 🌟 Overview
A mobile-first document processing pipeline that allows users to upload images or PDFs via Telegram and receive structured, cleaned data in return. This project solves the complexity of handling heterogeneous file types in a single stream.

### 🛠️ Technical Architecture
- **Type-Aware Routing:** Uses a logic switch to detect file MIME types (Image vs. PDF) and routes them to the correct processing engine.

- **JavaScript Post-Processing:** Custom JS snippets are used to clean OCR "noise" and format extracted text into a clean JSON structure.

- **Persistence Layer:** All extracted data is centralized into a Google Sheet for long-term accessibility.

### ⚙️ Tech stack
- **Primary Engine:** n8n (self hosted)
- **AI/LLM:** Gemini/OpenAI (AI Vision / OCR, text extraction)
- **Data & storage:** Google sheets 
- **Communication:** Telegram Bot API
