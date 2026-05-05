# 🚀 AdVantage Gen – AI Ad Creative Generator

AdVantage Gen is an AI-powered backend system that automates the creation of social media ad campaigns. It generates high-quality images, optimized captions, and platform-ready creatives from a single prompt.

---

## 📌 Overview

Modern marketing requires rapid experimentation and A/B testing. AdVantage Gen streamlines this process by generating complete ad creatives—including visuals, copy, and branding—within seconds.

Example Prompt:
"Eco-friendly coffee cup in a rainy cafe, focused on sustainability"

---

## ✨ Key Features

### 🎨 Multi-Modal Generation
- Generates **images** using Hugging Face (Flux/SDXL)
- Generates **captions + hashtags** using Gemini API
- Runs both processes **in parallel** for low latency

### 🖼️ Template Overlay & Branding
- Automatically overlays:
  - Brand Logo (with opacity control)
  - CTA buttons (e.g., *Shop Now*)
- Uses **Sharp / Canvas** for image compositing
- Outputs **ready-to-publish creatives**

### 🧠 Brand Voice Tuning
- Supports multiple tones:
  - Witty 😄
  - Professional 💼
  - Urgent ⚡
  - Inspirational 🌟

### 📊 Campaign Optimization
- Prompt enhancement pipeline using LLM
- Converts simple prompts → detailed AI-optimized prompts

---

## 🛠️ Tech Stack

- **Backend:** Node.js, Express.js
- **AI APIs:** Gemini API, Hugging Face Inference API
- **Image Processing:** Sharp / Canvas
- **Database:** MongoDB
- **Storage:** Cloudinary (for media assets)
- **Tools:** Git, Postman, VS Code

---

## 🏗️ Architecture Workflow

1. User submits prompt  
2. Prompt enhancement via LLM  
3. Parallel execution:
   - Image Generation API
   - Text Generation API  
4. Image compositing (logo + CTA overlay)  
5. Final ad creative output  

---

## 📂 Project Structure

ad-creative-backend/
│── controllers/
│── routes/
│── services/
│── utils/
│── middleware/
│── config/
│── models/
│── server.js
│── package.json


---

## ⚙️ Installation & Setup

```bash
git clone https://github.com/your-username/ad-creative-backend.git
cd ad-creative-backend
npm install
npm start

---

 API Endpoints (Sample)

Method	       Endpoint	                 Description
POST     	   /generate-ad	         Generate full ad creative
POST	       /upload-logo	             Upload brand logo
GET	          /campaigns	            Retrieve saved campaigns

---

## 🚀 Future Enhancements

- 📊 Performance analytics dashboard  
- 🎯 AI-based ad performance prediction  
- 🌐 Multi-platform export (Instagram, LinkedIn, Facebook)  
- 🤖 Fine-tuned brand-specific LLM  

---

## 👩‍💻 Author

**Gobika P**

---

## 📄 License

This project is licensed under the MIT License.



