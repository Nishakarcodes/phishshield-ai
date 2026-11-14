# PhishGuard AI

AI-powered phishing detection for **HackNova Bhopal 2K26 (HN05, Phishing Detection System)**.

**Live demo:** https://phishshield-ai-two.vercel.app

## What it does
Paste a suspicious SMS, email or link. PhishGuard AI analyzes it with the Google Gemini API and returns:
- A verdict: **PHISHING**, **SUSPICIOUS** or **SAFE**
- A risk score from 0 to 100
- Red flags found in the message
- Simple safety advice

## How it works
1. The user pastes text on the website (`index.html`).
2. The page sends it to a Vercel serverless function (`api/analyze.js`).
3. The function calls the Google Gemini API and returns the result as JSON.
4. The page shows the verdict, score, red flags and advice.

The Gemini API key is stored as a Vercel environment variable, so it is never exposed in the code or the browser.

## Tech stack
- HTML, CSS, JavaScript
- Node.js (Vercel serverless function)
- Google Gemini API
- Vercel (hosting) and GitHub

## Disclosure
- Third-party tools and APIs: Google Gemini API, Vercel, GitHub.
- AI-generated code: Claude (Anthropic) was used as a coding assistant to help write the code.

## Author
Built by Nishakar as an individual participant.
