# TokoAI — PayPal AI Hackathon 2026

Participant: Maulana Abdan Sakur (solo)
Devpost account: sakurabdan48 (sakurabdan48@gmail.com)
Hackathon registration: confirmed 28 October 2026
Submission deadline: 13 November 2026, 03:00 WIB (20:00 UTC, 12 November 2026)

## What it is
TokoAI is a one-page web app that helps small sellers sell faster:
1. A seller enters a product name, keywords, price, and tone.
2. An AI-assisted generator turns those inputs into a polished sales description.
3. The product is shown to buyers, who check out with a PayPal button.

## How to run (demo)
```bash
cd paypal_hackathon
python3 -m http.server 8000
```

Then open http://localhost:8000/ in a browser.

## PayPal Sandbox
- This demo uses the participant's own PayPal Developer Sandbox Client ID, so the PayPal button renders a full Sandbox checkout.
- No real money moves. For a full Sandbox checkout, log in with a Sandbox buyer account from PayPal Developer.
- The demo client-id `sb` in `index.html` has been replaced with the participant's own Sandbox Client ID from their PayPal Developer account.

## AI in this app
The description generator calls a language model at runtime: when the seller clicks "Generate description with AI", the app sends the product name, keywords, price, and tone to the Pollinations text API (a hosted LLM, keyless — no API key is stored anywhere) and displays the AI-written description. If the AI service is unreachable, the app falls back to a clearly labelled template draft so the demo still works offline. The AI call happens inside the finished app, every time a description is generated — it is not only a build-time tool.

## What is still needed for a complete Devpost submission
- [ ] Public GitHub repository containing this code (requires the participant's GitHub account)
- [ ] Demo video under 3 minutes, hosted on YouTube or Vimeo (Devpost asks for a video link)
- [ ] Create a Project in Devpost, with description, repository link, and video link
- [x] Replace the demo client-id with a PayPal Developer Sandbox Client ID for a full Sandbox checkout
