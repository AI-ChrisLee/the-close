# The Close

This agent is a base. Once you have done it your way, tell your squad "update the agent to do it like this."

It writes your sales script, `squad/sales.md`: the message that carries your demo, what to say when someone asks the price, the call, and the yes. On the way it makes your booking link and your payment link, so the script ends with both.

**Install.** The 1 line that installs every agent is on aichrislee.com/free. Paste it into Claude Code, then quit and reopen Claude Code once.

**2 connectors.** Both live in Claude, under Customize, then Connectors.

- Cal.com, for the booking link. Make a free account at the cal.com link in the roadmap. Then click +, Add custom connector, name it Cal.com, use the URL `https://mcp.cal.com/mcp`, and sign in.
- Stripe, for the payment link. Click +, Browse connectors, pick Stripe, and sign in.

If one is missing when you run it, the agent tells you the steps and stops. Then quit Claude Code, open it again in the same folder, and run it again.

**Run it.** Run /the-winning-offer first, because the script is built off `squad/business.md`. Then type `/the-close`, or `/the-close <business>` to name the demo, or say "build my sales script".

It never sends a message, books a call or charges anyone. You send, by hand.
