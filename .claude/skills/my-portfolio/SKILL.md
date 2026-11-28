---
name: my-portfolio
description: The user's personal investment portfolio, kept in their private Claude Doc "התיק שלי". Use this whenever the user talks about their portfolio ("התיק שלי"), their stocks or ETFs, whether to buy or sell something, sends a screenshot of their broker app, asks what market news means for them, or asks what to do with spare cash, even if they don't say "portfolio". Read the doc before giving any portfolio-specific view, so the answer continues from what was already decided.
---

# My portfolio

The portfolio data (holdings, cash, agreed rules, target allocation, open questions, upcoming events and the trade log) lives in the user's private Claude Doc, not in this repository, because the repository is public:

https://claude.ai/artifact/WV4BpXKw6qBhtMWJrBPk2Y

## Every time

1. Read the doc with the Claude Docs tools (load the docs skill or the docs connector's guide first). Never put the doc's contents into this repository, an artifact or any other external place.
2. Answer in Hebrew, short and scannable, verdict first; the user reads on a phone.
3. Apply the agreed rules in the doc instead of re-arguing them. If news genuinely changes the case for a rule, say so and let the user decide.
4. The doc's prices are a dated snapshot. Ask for a fresh broker screenshot (Holdings and Cash Balance) before quoting weights, or say you're using the snapshot.
5. Get market facts from a search, and say when a figure comes from a single source.
6. Say once, briefly, that this is not financial advice when you suggest a trade.

## When the user sends an order screen

Check Buy/Sell, quantity, Limit order type, the limit versus Bid/Ask, Duration Day, Market Hours Regular, and that the total fits the USD cash balance (Buying Power includes a credit line the user doesn't want to use).

## After a confirmed trade or decision

Update the doc: holdings table, cash, the as-of date, and a new row at the top of the trade log (date, action, price, reason). Edit only what changed.
