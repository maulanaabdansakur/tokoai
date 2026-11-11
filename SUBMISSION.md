# Devpost submission draft — TokoAI

## Title
TokoAI — AI Product Descriptions + PayPal Checkout for Small Sellers

## Tagline
Sellers type a product name and keywords, AI writes the sales description, buyers pay with PayPal.

## Description
Small sellers often lose sales because writing a good product description takes time and feels hard. TokoAI removes that friction: a seller enters a product name, a few keywords, a price, and a tone, and the app generates a clear, ready-to-use sales description in seconds. The product is then shown to buyers on the same page, with a PayPal checkout button, so a seller can go from an idea to a sellable listing and a payment in one flow.

The demo runs on PayPal Sandbox, so no real money moves during testing. The app is built as a single, fast web page, so it works on a phone browser without installation.

## How it uses PayPal
Buyers check out with the PayPal JavaScript SDK in Sandbox mode. In the final version, the demo client-id is replaced with the participant's PayPal Developer Sandbox Client ID, and checkout is completed with a Sandbox buyer account.

## How it uses AI
The app calls a language model at runtime: when a seller clicks "Generate description with AI", the app sends the product name, keywords, price, and tone to the Pollinations text API (a hosted LLM, keyless — no API key stored in the code) and the model writes the sales description, which is shown on the page and then published to buyers. If the AI service is unreachable, the app falls back to a clearly labelled template draft so the demo still works offline.

## Built with
HTML, CSS, JavaScript, PayPal JavaScript SDK (Sandbox)

## Links to add before submitting
- GitHub repository: [TO ADD — public repo link]
- Demo video (under 3 minutes): [TO ADD — YouTube/Vimeo link]
