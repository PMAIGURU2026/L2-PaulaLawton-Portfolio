# January 2026 — AI-Powered Web Application

**Month:** January 2026  
**Program:** Pursuit AI Fellowship — Level 2  
**Author:** Paula Lawton

---

## Description

This project brings AI capabilities into a user-facing web application. Using React for the frontend and a Python/Flask backend, the app integrates with the OpenAI API to deliver an interactive AI assistant. The focus was on full-stack development patterns, API design, and responsible AI practices (rate limiting, content moderation, user feedback loops).

## Topics Covered

- RESTful API design with Flask
- Frontend development with React (hooks, state management, async/await)
- Integrating third-party AI APIs (OpenAI Chat Completions API)
- Environment variable management and secrets handling
- Prompt engineering fundamentals
- CORS, error handling, and loading states in full-stack apps

## Project Highlights

- **AI Study Assistant:** A web app where users can paste a study topic or document excerpt and ask follow-up questions. The Flask backend forwards requests to the OpenAI API with a carefully crafted system prompt to keep responses educational and concise.
- **Prompt Engineering Experiments:** Documented experiments comparing zero-shot, few-shot, and chain-of-thought prompting strategies on the same input, with qualitative evaluation of outputs.
- **Rate Limiting Middleware:** Implemented a simple token-bucket rate limiter on the Flask backend to prevent API cost overruns.

## Skills Demonstrated

- Building and deploying a full-stack AI application
- Secure handling of API keys using `.env` files (never committed to version control)
- Writing clear, focused system prompts to steer model behavior
- React component architecture and state management

## How to Run

```bash
# Backend
cd backend
pip install flask flask-cors openai python-dotenv
cp .env.example .env   # Add your OPENAI_API_KEY
python app.py

# Frontend (separate terminal)
cd frontend
npm install
npm start
```

> **Note:** You will need a valid OpenAI API key to run this project.

## Key Takeaways

Shipping an AI feature is less about the model and more about product design: what context to pass, how to handle errors gracefully, and how to set user expectations. Prompt engineering is a real skill that requires iteration and evaluation.
