# 🏗️ Design Document — The Zero-Waste Chef

> *A Multimodal AI System for Rebuilding Meals from Existing Ingredients*

---

## 📌 1. System Overview

**The Zero-Waste Chef** is an AI-powered mobile application that transforms images of fridge or pantry contents into intelligent, waste-minimizing recipes.  
The system combines **computer vision**, **multimodal LLMs**, and **agentic workflows** to eliminate *fridge paralysis* and promote sustainable cooking.

---

## 🧠 2. Design Goals

- Convert ingredient images into accurate inventories
- Generate recipes using **only available ingredients**
- Prioritize perishable items
- Prevent AI hallucinations
- Quantify environmental and financial impact
- Ensure a smooth, intuitive user experience

---

## 🏛️ 3. High-Level Architecture

<p align="center">
  <img src="high_level.png" alt="High level architecture" width="200" height="300">
</p>

---

## 🧩 4. Core Components

### 📱 Mobile Application
- Image capture & upload
- Ingredient confirmation UI
- Step-by-step cooking mode
- Impact visualization dashboard

### ⚙️ Backend API
- Handles image uploads
- Manages sessions & orchestration
- Connects AI services
- Returns structured responses

### 👁️ Computer Vision Engine
- Ingredient detection
- Food classification
- Quantity approximation

### 🧠 Agentic Reasoning Engine
- Validates ingredient list
- Applies perishable-first logic
- Enforces strict constraints
- Eliminates hallucinated ingredients

### 🍳 Recipe Generation Engine
- Multimodal LLM-based
- Cuisine-aware recipe creation
- Structured, readable output

### 🌍 Impact Analytics Engine
- CO₂ emission savings calculation
- Estimated grocery cost savings

---

## 🔄 5. Data Flow

1. User uploads fridge/pantry image  
2. Backend receives image  
3. Vision model extracts ingredients  
4. User confirms or edits list  
5. Agent prioritizes perishables  
6. Recipe is generated  
7. Impact metrics calculated  
8. Results displayed to user  

---

## 🧰 6. Technology Stack

| Layer | Technologies |
|-----|-------------|
| Frontend | Flutter / React Native |
| Backend | FastAPI (Python) |
| AI Models | Gemini / GPT (Multimodal) |
| Vision | Custom CV models |
| Agent Framework | LangChain / CrewAI |
| Database | Supabase / PostgreSQL |
| Impact APIs | Carbon & Pricing APIs |

---

## 🔐 7. Security & Privacy

- HTTPS-based communication
- Secure handling of image data
- No permanent image storage by default
- Encrypted user data storage

---

## ⚡ 8. Performance & Scalability

- Asynchronous request handling
- Horizontally scalable backend
- Cached recipe lookups
- Optimized image processing pipeline

---

## ⚠️ 9. Known Limitations

- Ingredient detection depends on image quality
- Carbon calculations are estimations
- Limited cuisine coverage in initial version

---

## 🚀 10. Future Enhancements

- Smart fridge integration
- Personalized nutrition goals
- Community recipe sharing
- Offline cooking mode
- Multilingual support

---

## ✅ Summary

This design demonstrates how **multimodal agentic AI** can convert everyday kitchen activity into a powerful sustainability solution—bridging the gap between intention and action.

---


