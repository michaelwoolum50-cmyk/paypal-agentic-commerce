# PayPal Agentic Commerce Agent

**Tell it what to do with money in plain English. It handles the PayPal.**

An autonomous agent that manages PayPal payments through natural language — creating invoices, splitting bills, tracking what's owed, settling up — powered by a local open-source LLM with the PayPal API as its hands.

*Entry for the PayPal AI Hackathon ($69,750 prize pool) — targeting "Best Use of Agentic Commerce" ($5K) + overall placement.*

## Concept

```
You: "Invoice Sarah $200 for the logo work, due Friday"
Agent: → PayPal Invoicing API → invoice created → "Done. Invoice #INV-2041 sent to Sarah, due Friday."

You: "Split last night's $180 dinner three ways"
Agent: → creates 2 invoices → "Sent $60 requests to Mike and Jen."
```

## Architecture

- **Brain:** Qwen 2.5 Coder 7B (local, open-source) — parses intent, plans API calls
- **Hands:** PayPal REST API (Invoices v2, Payouts) via sandbox → production
- **Memory:** local SQLite ledger of every invoice, payment, and settlement

## Status

🚧 **In build** — repo staged for the hackathon. Deadline: November 12, 2026.

## Requirements (per hackathon rules)

- [ ] Meaningful PayPal integration (Invoicing + Payouts API)
- [ ] Working demo
- [ ] Public GitHub repo (this one)
- [ ] Demo video ≤3 min
