---
name: execution-genesis-close
description: Use this when the founder needs the sales script and the booking and payment links, when they type "/execution-genesis-close" or "/execution-genesis-close <business>", or say "build my sales script". It makes a 30-minute booking link through their Cal.com connector and a payment link at their own price through their Stripe connector, then writes squad/sales.md with both links on the last line. It never sends, books or charges.
---

# execution-genesis-close

1 output: `squad/sales.md`, the sales script, with a real booking link and a real payment link on its last line.

**The first message of a fresh run** (no `squad/sales.md` on disk) carries this line, word for word:

> This agent is a base. Once you have done it your way, tell your squad "update the agent to do it like this."

Open `references/the-script.md` first. Missing: say the agent folder came without its `references/`, and stop.

## 1. Read

- `squad/business.md`. Missing: say "Run /execution-genesis-offer first. Your sales script is built off that page." and stop.
  Take THE SENTENCE, WHO line 1, THE PROBLEM, THE PROMISE, PRICE line 1 and BUYER WORDS.
- `squad/demos/*/facts.md`. The buyer is the folder the founder names (`/execution-genesis-close maple-family-dental`), else the folder whose `facts.md` changed last. Say which in 1 line: `Writing it for <business>.`
  Take FIRST NAME, his business, his facts, and the `LOOM <url>` last line. No demo yet: those stay blanks.
- `.claude/squad-roots.md`: the founder name, the voice sample, the `product word` row. No founder name: the name `get_me` gives. No voice sample: short plain sentences.

## 2. Check the connectors

Look at the loaded tools before you make anything. A connector is needed only for a link the last line of `squad/sales.md` does not carry yet.

- Cal.com is loaded when tools ending in `get_me`, `get_event_types` and `create_event_type` are on the list.
- Stripe is loaded when tools ending in `get_stripe_account_info` and `stripe_api_write` are on the list.

1 missing: print its message below, word for word, and stop. Both missing: print the Cal.com steps, then the Stripe steps, with "Then quit Claude Code, open it again in this folder, and type /execution-genesis-close again." once at the end. Nothing is made until every connector needed is loaded.

**Cal.com not loaded:**

```
Your booking link needs Cal.com, and it isn't connected yet. 4 steps:
1. Make a free cal.com account at the cal.com link in the roadmap.
2. In Claude, click Customize, then Connectors, then +, then Add custom connector.
3. Name it Cal.com. URL: https://mcp.cal.com/mcp
4. Click Add, then sign in to Cal.com.
Then quit Claude Code, open it again in this folder, and type /execution-genesis-close again.
```

**Stripe not loaded:**

```
Your payment link needs Stripe, and it isn't connected yet. 2 steps:
1. In Claude, click Customize, then Connectors, then +, then Browse connectors, and pick Stripe.
2. Click Connect, then sign in to Stripe. No Stripe account yet? Make a free one at stripe.com, then sign in.
Then quit Claude Code, open it again in this folder, and type /execution-genesis-close again.
```

## 3. The booking link

1. `get_me`: the username, and the name when the roots file has no founder name.
2. `get_event_types`: an event type titled `Call with <founder name>` is reused. Never make a second one.
3. None: `create_event_type` with title `Call with <founder name>`, slug `call-with-<founder name>` lowercased with hyphens, `lengthInMinutes` 30.
4. The booking link is the event type's `bookingUrl`. No `bookingUrl` in the reply: `https://cal.com/<username>/<slug>`.

## 4. The payment link

Stripe's tool names change. Read the live Stripe tool list and use only what is on it.

1. `get_stripe_account_info`: the account's default currency, and whether it can take real money yet (`charges_enabled`).
2. PRICE line 1 without its words in parentheses decides what gets made, the same numbers and nothing else:
   - `one-time`: 1 price, charged once.
   - `a month`: 1 price, recurring every month.
   - `setup + $N a month`: 2 prices on the same link, the setup number charged once and $N recurring every month.
3. Before each write, read that method's live parameters with `stripe_api_details`. Then, through `stripe_api_write`, in this order:
   - **The product.** Name: the `product word` row, else the noun of THE SENTENCE. List the active products with `stripe_api_read` first; one with this exact name is reused, with any active price that has the same amount, currency and term.
   - **The price.** `unit_amount` in cents (`$1,500` is `150000`), the account's currency, and `recurring[interval]` = `month` on a monthly one.
   - **The payment link.** `line_items`, each price at quantity 1.
4. The payment link is the reply's `url`.

Not able to take real money yet (`charges_enabled` false, `livemode` false, or `test_` in the url): say it in 1 line, "This link won't take real money until Stripe verifies your business." A sandbox link carries `test_`; a live one starts `https://buy.stripe.com/`.

## 5. Write the script

Write `squad/sales.md` whole, to `references/the-script.md`, section by section, to its law. Every line comes from `squad/business.md`, the demo's `facts.md`, or that file. The last line is exactly `Book: <booking url>. Pay: <payment url>.` and nothing comes after it.

Check before you save:

- The price is said once, in THE CALL, and it is PRICE line 1 without its words in parentheses. No other money number anywhere.
- No price in THE MESSAGE or HOW MUCH.
- No discount, no payment plan, no guarantee, no money he will make.
- No fact about the buyer that is not in `facts.md`. A blank stays a blank.
- No em dash, and the bold lines sound like the voice sample.

## 6. Print

The path `squad/sales.md`, then 3 lines off the file, never the whole file:

1. The message.
2. The price line.
3. The client 2 line.

Then: "Change any line by telling me what it should say."

A change: rewrite that line only. A new number goes through /execution-genesis-offer, because this file only carries PRICE.

## Typed again

- The links on the `Book:` and `Pay:` last line are reused, never made twice.
- PRICE line 1 no longer matches the price line: make a new payment link for the new PRICE (step 4), update the price line and the `Pay:` link, and say so in 1 line.
- Rewrite THE MESSAGE and CLIENT 2 for the buyer from step 1. Every other section stays as it is on disk.
- The founder names who sent this buyer: THE MESSAGE opens with "<that name> just started with me and said you have the same problem."

## Never

- Send, post, book or charge anything. The founder sends the message by hand and sends the payment link himself, on the call.
- A price that is not PRICE line 1, a range, a discount or a payment plan.
- A guarantee, or a promise of money he will make.
- An invented fact about the buyer, an invented win, or an invented quote.
- A second booking link or payment link when the last line already carries one.
- Print a key or a token.
- Write any file but `squad/sales.md`.
