# smartmail-ai-writer
SmartMail AI Assistant is an intelligent email-reply automation system that integrates with Gmail, React, and Spring Boot, leveraging Google’s Gemini AI model to generate context-aware, professional email replies instantly

🚀 SmartMail AI Assistant

AI-powered Email Reply Generator using Spring Boot, React, and Google Gemini API

SmartMail AI Assistant is an intelligent email automation tool that generates professional email responses based on user-provided content.
It integrates Gmail (via Chrome Extension), React frontend, Spring Boot backend, and Google Gemini LLM.

📌 Table of Contents
Overview:
-Features
-Architecture
-Tech Stack
-Project Workflow
-Folder Structure
-Backend (Spring Boot)
-Frontend (React)
-Chrome Extension
-Environment Variables
-API Endpoints
-How to Run the Project
-Screenshots
-Future Enhancements
-Author


🧠 Overview

SmartMail AI Assistant is a full-stack AI automation system that generates email replies using the Google Gemini Generative Language API.

It supports:

Manual email generation via frontend

API-based usage (Postman, external clients)

Gmail auto-detection via Chrome Extension

Quick insert of generated replies in the Gmail compose box

⭐ Features
🔹 AI-Generated Email Replies

Uses Google's Gemini model (gemini-2.5-flash) to generate high-quality email replies.
🔹 Tone Customization
Choose tone:
Professional
Casual
Friendly

🔹 React Frontend + Live Preview
Users can input original email, choose tone, and view generated reply instantly.
🔹 Chrome Extension for Gmail
Automatically detects Gmail compose window and injects an AI Reply button.
🔹 Complete Backend API
Spring Boot REST API endpoint for generating responses.
🔹 CORS Enabled
Full support for communication between React & Spring Boot.

🏗 Architecture:
React UI  →  Spring Boot Backend  →  Google Gemini API
       ↳ Chrome Extension → Backend API → Gemini


🛠 Tech Stack
Frontend
React.js
JavaScript
Material UI
Axios

Backend
Spring Boot (3.x)
WebFlux (WebClient)
Lombok
Jackson

AI
Google Gemini Generative Language API

Browser Extension
Manifest V3
JavaScript DOM events
MutationObserver API

🔄 Project Workflow

User enters email content (React UI or Gmail compose window)
React / Extension sends request → Spring Boot
Backend builds prompt & calls Gemini API
Gemini model returns AI-generated email reply
Reply is displayed to user OR inserted automatically into Gmail



