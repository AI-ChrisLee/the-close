# Answering a reply: the buckets, the door, the drafts

REPLY mode reads this file before sorting a batch and before printing one. It carries how a reply
gets bucketed, which door the interested ones get, and what every draft has to survive. It wins
over any memory of the buckets, and this file and the skill change in one edit.

Every reply gets one bucket, with the reason written next to it in the founder's own terms so
they can disagree with it. **The Status column is not a judgment call:** the bucket decides it,
because that column in the Warm CRM moves one way only and a guessed value is expensive to undo.

| Bucket | What it sounds like | The move | The next touch | Status |
|---|---|---|---|---|
| Interested | "send the link", "let's talk", "when can you start" | One next step, this hour | Link sent: day 4, one nudge if the money has not cleared, then stop. Call booked: the call itself, nothing else scheduled | `TALKING` |
| Question | "how much", "do you do X", "how long" | Answer from the card, ask one back. A priced question whose scope fits one sentence is interested instead, and gets the way to pay | Day 4, one bump, then the not-now shelf | `TALKING` |
| Objection | "too expensive", "we have someone", "we'd just use AI" | Test it, never answer it | Day 4, one bump; if they named the real blocker, the date it clears | `TALKING` |
| Not now | "after the summer", "we're mid-launch" | Get the date in their words | The date they gave, quoted; no date given, ask for one | `NOT NOW` |
| No | "not interested", "remove me", anything hostile | One line, the shortest in the batch, row closed | None, ever | `CLOSED` |

A reply with no ask in it gets no bucket and stays in the warm morning; its row still moves to
`TALKING`, because a person who answered is a person you are talking to. `DEMO SENT` belongs to
the Warm Start and never gets written from a reply.

## Tiebreaks, so the same reply always lands the same way

- **A yes is a commitment carrying a next step:** send it, let's talk, when can you start.
  Might, maybe and possibly are a **question**, and the draft asks the one thing that turns the
  maybe into a date.
- "Send me more information" is a question. One paragraph and one question back, never an
  attachment.
- A handoff inside their own company (talk to my partner, email our ops lead) is **interested**,
  and the draft asks for the introduction instead of pitching the new person cold. **A name
  somewhere else is a referral, not this deal:** the draft thanks them and asks for the
  introduction, and the new name goes back to the Warm Start as an A row with the referrer
  written into its HOW YOU KNOW THEM line. A referred name is the strongest row on any list.
- A reply that names an incumbent and asks a real question is a **question**, not an objection.
  Answer it from the card in one line first, then ask the test question second. "We have an
  editor already but he is slow, what would you do different" is somebody asking to be sold to,
  and testing it before answering it reads as a dodge.
- A price complaint from somebody who was never given a price is an **objection** about value.
  From somebody who was never pitched at all it is a conversation: one question back, and it
  stays in the warm morning.
- **An auto-reply is not a reply.** An out of office carries no ask, so it gets no bucket and no
  draft, and it never counts in the day's replies number. It still gets a row write: move that
  person's next touch to the day after the return date they gave, quoted in their words, and
  leave Status where it stands. A return date nobody wrote down is a person who gets messaged
  while they are away.

## The door, for the interested ones only

Printed as one word plus a one-line reason so the founder can flip it. The **link** when the card
carries the price and the scope fits one sentence; the **call** when either one is fuzzy. The
link message is the payment path, that one sentence of scope, a start date, and an invitation to
raise anything before paying. The call message carries the booking link off the client page and
says what the call decides, including that a number arrives before they hang up. **Neither link
exists yet: the door is the call, and the message asks for their two best times instead of
offering yours.** Answer a money question with a way to pay, never with a calendar. What happens
on the call belongs to phase 2, not to the draft.

## What every draft has to be

Short enough to have been typed on a phone, carrying one ask, quoting their own words back, and
**never discounting.** Objections get tested and not answered, the same move as block 4.

**The gate, before the batch prints.** Read every draft back against three fail conditions, and a
draft that trips one gets rewritten rather than shown: a number the offer card does not carry, a
second ask anywhere in the message, a claim that is not in the credibility bank. Say which drafts
were rewritten and why. A batch that goes out carrying one of those three costs the founder the
deal it was written for.

## After it goes out

One bump, counted day 4 from the message that went out, and nothing after it. **A reply retires
that person's unsent warm touches,** because those were written for silence: strike the day 4 and
day 9 touches in `squad/warm/drafts/NN-firstname-lastname.md` by name, and say in one line that
you did. The draft file stops being the schedule the moment they answer, and a touch left
standing in it fires on top of this thread the next warm morning. Nobody gets two messages in one
day.
