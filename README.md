# IBM-Circuit-Buddy-AI-Chatbot

# Chatbot - Audio Signal Processing Assistant Agent

[![Audio Signal Processing](https://img.shields.io/badge/Audio%20Signal%20Processing-blue)](https://github.com/topics/audio-signal-processing)
[![AI Chatbot](https://img.shields.io/badge/AI%20Chatbot-lightgrey)](https://github.com/topics/chatbot)
[![IBM Granite](https://img.shields.io/badge/IBM%20Granite-green)](https://github.com/topics/ibm-granite)
[![IBM Cloud Lite](https://img.shields.io/badge/IBM%20Cloud%20Lite-blueviolet)](https://github.com/topics/ibm-cloud)
[![Electronics Engineering](https://img.shields.io/badge/Electronics%20Engineering-orange)](https://github.com/topics/electronics-engineering)


---

**A cloud-native AI chatbot that assists students, engineers, and hobbyists with designing and troubleshooting audio circuits.**  
_Built with IBM Granite 3-3-8b-instruct and deployed on IBM Cloud Lite._

## 🚀 Overview

The Audio Signal Processing Assistant Agent is an expert AI assistant that helps users:
- Diagnose and resolve common issues in audio circuits (preamps, filters, amplifiers, etc.).
- Provide step-by-step troubleshooting, noise reduction, and distortion elimination advice.
- Offer best practices and design recommendations (filter selection, component values, grounding, PCB layout).
- Answer technical questions and explain concepts for both analog and digital audio signal processing.

Built using state-of-the-art large language models (LLMs) and retrieval-augmented generation (RAG), the agent provides fast, accurate, and context-aware support in real time.

## 🛠️ Features

- **Technical Troubleshooting**: Answers questions like “Why is my audio amplifier producing noise?” or “How do I reduce distortion in my op-amp circuit?”
- **Design Guidance**: Suggests filter designs, amplifier configurations, and optimal layout/grounding strategies.
- **Retrieval-Augmented**: References a curated database of FAQ pairs, best practices, and expert documentation for reliable answers.
- **Cloud Hosted**: Powered by IBM Cloud Lite—no local install or compute required.
- **Always-On and Scalable**: Accessible from anywhere via web or API.

## 📊 Technologies Used

- **IBM Granite 3-3-8b-instruct**  
  Instruction-tuned large language model (LLM), optimized for technical dialog and Q&A, hosted via IBM Cloud Lite.
- **IBM Watsonx/Granite SDK & API Client**  
  For secure access to AI model endpoints and deployment.
- **Langchain**  
  For orchestration, context management, memory, and tool plugin support.
- **Retrieval-Augmented Generation (RAG)**  
  For injecting accurate, domain-specific knowledge into AI answers.
- **Knowledge Base**  
  Curated, preprocessed Q&A pairs, technical guides, and audio engineering documents.

## 🔧 System Requirements

- **User**: Any device with web browser and Internet access.
- **Backend**: Runs entirely on IBM Cloud Lite (GPU/cloud compute provided).
- **Development**: Python 3.8+, with the following libraries:
  - `ibm_watsonx_ai`
  - `langchain_ibm`
  - `pandas`, `numpy`
  - `json`, `requests`

## 🗂️ Data & Model Pipeline

1. **Data Collection**  
   - General technical documents, books, and web articles.
   - Domain-specific: audio circuit FAQs, troubleshooting guides, filter design references.
2. **Preprocessing**  
   - Text cleaning, tokenization, deduplication, quality filtering, and structured QA formatting.
3. **Model & Retrieval**  
   - LLM inference performed on Granite with RAG pipeline injecting most relevant knowledge base documents for grounded answers.
4. **Prediction/Interaction**  
   - User queries are processed, context is retrieved, and the model returns detailed, actionable technical guidance.

## 🧑💻 How to Use

1. **Ask a Question**:  
   Submit your query (e.g., “My preamp is humming loudly. What should I check?”).
2. **Get Instant Support**:  
   The agent responds with targeted advice and troubleshooting steps.
3. **Follow Up**:  
   Continue the conversation for deeper diagnostics, recommended circuits, or step-by-step design help.

## 🚩 Example Interactions

> **User:** _Why is my op-amp circuit distorting at high volumes?_  
> **AI Agent:** _Distortion can be caused by op-amp slew rate limitations, low supply voltage, or input overdrive. Try increasing supply voltage within device specifications, reducing input amplitude, or choosing a higher-bandwidth op-amp._

> **User:** _Can you help me design a 2kHz low-pass filter?_  
> **AI Agent:** _Absolutely! For a Sallen-Key low-pass filter with 2kHz cutoff: try R=8kΩ, C=10nF, or use RC=1/(2πf). Let me know if you want an active or passive design._

## 🔒 Security & Deployment

- All computation and model inference run securely in the IBM cloud.
- Data privacy is maintained—no user questions or personal data is stored locally unless logging is explicitly enabled for research/development.

## 📈 Future Scope

- Expand the knowledge base with advanced topics (DSP, digital filters, simulation).
- Add support for schematic/image input and analysis.
- Integrate circuit calculators and design plugins for deeper design automation.
- Multi-language and voice support.

## 📚 References

- [IBM Granite Model Docs] (official documentation)
- Audio Engineering Society Publications
- Standard electronics and circuit design manuals
- Open-source LLM literature

## 🤝 Contributing

Contributions, feedback, or new Q&A/document additions are welcome! Please submit an issue or pull request.

## 📜 License

_MIT License (or specify your chosen license)_  
**Copyright (c) 2025 [U Chethan Raj/Team]**

