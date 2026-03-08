# 🎙️ Speechify: Learning Companion Mode
### Pursuit AI Fellowship — Level 2 | Week 4 Team Project
### Built by: Paula Lawton (Product Lead) + David O (Technical Lead)
### Date: February 14, 2026

## What It Does
A Speechify clone that transforms passive audio listening into
active learning. AI generates comprehension quizzes every 5 minutes
during playback, tracks your answers, and shows your retention
score over time on a personal dashboard.

## Why We Built It
Audio learners retain only 20% of content they passively hear.
With active recall (quizzes), retention jumps to 80%.
Learning Companion Mode bridges that gap.

## Frontend Stack
- React.js v18+
- Tailwind CSS
- React Router
- Axios (API calls)
- React Speech Kit / Web Speech API (TTS = Text-to-Speech)
- Deploy: Vercel or Netlify

## Backend Stack
- Node.js + Express.js
- OpenAI API (GPT-4) — quiz generation engine
- PostgreSQL / Supabase (database)
- JWT (JSON Web Token) — user authentication
- Deploy: Render.com or Railway

## Database Tables
- users — accounts + subscription tier
- listening_sessions — content + duration tracking
- quiz_attempts — questions, answers, correct/incorrect, timestamps

## Business Model
- Free Tier: 10 min/day listening, 3 quizzes/day
- Premium: $139/year — unlimited listening, 30+ voices, analytics

## My Contributions 🌟
- 📋 Product Manager (PM) — wrote the full PRD + all framework
  analysis (RICE, KANO, MoSCoW, Value vs. Effort Matrix)
- 💻 Frontend Developer — built audio player + quiz UI
- 🤖 AI Integration — OpenAI quiz generation logic
- 📊 Presentation — built Demo Day pitch deck slides
