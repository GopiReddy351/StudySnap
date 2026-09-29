# StudySnap 📚
Snap a picture of tricky homework, diagrams, or handwritten notes, and get clear step-by-step explanations in seconds. Send your study cheat sheets straight to WhatsApp when you're done.

# What is StudySnap?
Ever get stuck on a textbook problem or a messy equation at midnight with nobody around to explain it?

StudySnap is an AI-powered study buddy designed to turn photos of textbook pages, handwritten worksheets, or typed questions into plain-English, step-by-step explanations. Instead of dumping a wall of text or overly complex jargon, it isolates the problem, provides the direct answer, and walks through the solution logic simply.

Once your study session wraps up, StudySnap bundles everything you worked on into a clean, text-friendly recap and sends it directly to your phone via WhatsApp so you have a quick cheat sheet for review.

# Key Features
Snap to Solve: Upload a photo of handwritten notes, print worksheets, or diagrams (powered by multimodal vision models).

Zero Jargon Explanations: Clean, conversational breakdowns that emphasize how to solve the problem, not just the final number.

Strict Academic Guardrails: Tuned specifically to keep students on track—politely deflects off-topic banter back to the study material.

WhatsApp Session Recaps: Export your entire session's formulas, takeaways, and solved questions into an emoji-friendly, copy-pasteable WhatsApp message.

# Tech Stack
Backend: Python (FastAPI / Flask)

AI Core: Google Gemini API / OpenAI GPT-4o (Vision & Multimodal inference)

Messaging Integration: Twilio WhatsApp API / Meta Cloud API

Environment & Config: python-dotenv

# Project Structure
Plaintext
studysnap/
│
├── app.py                # Main application entry point & API endpoints
├── prompts.py            # System prompts, templates, and persona definitions
├── services/
│   ├── vision_service.py # Image processing & LLM query logic
│   └── whatsapp.py       # WhatsApp messaging and recap dispatcher
├── .env.example          # Environment variables template
├── requirements.txt      # Python dependencies
└── README.md
Getting Started
# Prerequisites
Python 3.10+

An API key for an LLM vision provider (e.g., Gemini API, OpenAI)

A Twilio account or Meta Developer App (for WhatsApp messaging)
