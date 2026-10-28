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
- This demo uses the PayPal Sandbox demo client-id `sb`, so the PayPal button renders without a personal Client ID.
- No real money moves. For a full Sandbox checkout, log in with a Sandbox buyer account from PayPal Developer.
- For the final submission, replace `client-id=sb` in `index.html` with the Sandbox Client ID from the participant's PayPal Developer account.

## AI in this prototype
The description generator in this prototype is rule/template-based: it builds benefits, selling points, and a call to buy from the seller's inputs, in the selected tone. It runs without an API key so anyone can test the demo.
For a stronger final version, replace that function with a language-model (LLM) API call, with the API key kept securely on a server, not in the HTML file.

## What is still needed for a complete Devpost submission
- [ ] Public GitHub repository containing this code (requires the participant's GitHub account)
- [ ] Demo video under 3 minutes, hosted on YouTube or Vimeo (Devpost asks for a video link)
- [ ] Create a Project in Devpost, with description, repository link, and video link
- [ ] Replace the demo client-id with a PayPal Developer Sandbox Client ID for a full Sandbox checkout
