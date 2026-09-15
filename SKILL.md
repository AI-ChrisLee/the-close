---
name: the-close
description: Use this when money enters a conversation, by inbox or by call. The founder says "/the-close script", "I just got off a call with ____. Here is the transcript: ____" (pasted, or a path to it or to the recording), or pastes a reply and says "sort this reply". It builds squad/sales.md, the one sales script everything they say for money comes out of, grades every call against 4 gates with the evidence quoted, files the debrief, writes what the call taught back into the script, and logs the pipeline row. It never sends anything.
---

# The Close

The Winning Offer built the offer document. This skill sells it: one general sales script at `squad/sales.md`, sharper after every call.

**First message on a fresh run** (no `squad/sales.md` on disk), say this line first: This skill is a base. Once you have done it your way, tell your squad "update the skill to do it like this."

**You never send.** No email, no DM, no booking, no payment link, nothing written into any calendar. You draft; their hand presses send.

Source order: the offer document `squad/business.md` (the promise, the warranty, the delivery day, the price), then the founder's 3 answers, then the buyer's own words in `squad/clients/<first-last>/notes.md`, which beat anything you write. You are last, and you invent nothing.

## Sources

This skill runs in any founder's repo. `.claude/squad-roots.md` is the per-repo instance file every member-run skill reads first (founder name, product word, and the `clients`, `sales` and `pipeline` rows where a run has written them), and its values win over the `squad/` paths below, which are worked examples. `<brand>` is the roots file's `product word` row, or the founder's own name when that row is missing. `<first-last>` is the folder the Winning Offer's warm entry already made for that person (matched on the first name when that is all the folder carries), firstname-lastname lowercased when none matches. `<date>` is `YYYY-MM-DD`.

Three files in this skill's folder must open, or the run stops and says the folder came without its `references/`: `references/sales-document.md`, `references/gates-and-rungs.md`, `references/reply-buckets.md`. Those files call the script build beat 1 and the after-a-call run beat 2.

Then read `.claude/squad-roots.md`, `squad/business.md` and every `squad/clients/*/notes.md`. No other source feeds the script.

No `squad/business.md`: no price to say, so point at g4 or g5. "sort this reply" still runs, with no number in any message. This skill never writes `squad/business.md`.

**What it writes, and nothing else:** `squad/sales.md` · `squad/clients/<first-last>/transcript.md` · `squad/clients/<first-last>/notes.md` · `squad/clients/<first-last>/calls/<date>-debrief.md` · `squad/pipeline.md` · the `sales` and `pipeline` rows in `.claude/squad-roots.md` (the `clients` row belongs to the Winning Offer's warm entry, never written here). Never `squad/calls/`, never `squad/offer-research.md`, never a per-person sheet, never a pre-call file, never a follow-up draft, never a calendar event.

## The script · `/the-close script`

One general script, never one per person. The founder opens it with a buyer on the line and runs it top to bottom.

Ask 3 things, in plain words, then build:

1. Your booking link, where a stranger books an hour.
2. Your payment link, a URL or a handle a stranger can pay by.
3. One win you can name, and how it happened. None yet is an answer.

Write `squad/sales.md` to `references/sales-document.md`, section by section, to its law. Nothing in it that is not that file's own lines, the offer document, those 3 answers, or the buyer quotes in `squad/clients/*/notes.md`. The price line is drafted off the offer document's PRICE line (its number, or the first rung of its ladder). The plan's last day is the day the offer document promises. The 3 rungs, FULL, MIDDLE and FLOOR, get decided here out of `references/gates-and-rungs.md`: what comes out if the number has to move, never the same thing for less money. Answer 3 is the proof line, marked `(founder's own)`; `(none yet)` runs the pitch on 3 beats.

Self-check before the stop: no angle bracket left in a spoken line, no one buyer's name or fact standing as a general line, no spoken line about what the founder has not built or done yet.

**The gate.** Say the path `squad/sales.md`, never print the file, then hold up 4 lines for the read:

- The open's agenda sentence, promising no more than the offer document does.
- The price line, its one number in it, never a price `squad/business.md` does not carry.
- Whose win the proof is. "Mine" is written as mine, and it is said as mine on the call.
- The plan in days, Day 1 and the offer document's promised day, never phase names. You never date a step the offer document or the founder did not say.

Fix what they change, then their yes. On yes, stamp the script's last line `confirmed <date>` and add the `sales` row to `.claude/squad-roots.md` when it carries none.

Typed again: read what is on disk and continue at the first thing missing, and a debrief or an objection parked with no script gets its writes the first time the script exists. A confirmed script is never rebuilt, and what it already answers is never re-asked. To change a line any time, the founder says the line and what it should read.

## After a call · "I just got off a call with ____. Here is the transcript: ____"

Runs the moment the call ends.

What it takes: a paste, or a path to `.txt`, `.md`, `.srt`, `.vtt`. A recording (`.m4a`, `.mp3`, `.wav`, `.mp4`, `.mov`) is transcribed on the laptop by `the-winning-offer/references/recording.md`, next to this skill's folder; that file missing, say so in one line and ask for a transcript instead. Nothing uploads. An app-written transcript is marked rough in the debrief. Notes only: gates 1 and 2 are graded on the founder's estimate, the debrief says so, and every buyer line off the notes is labeled `(founder's recollection · Name · date)`. Nothing at all: ask what happened, in plain words.

Save what landed to `squad/clients/<first-last>/transcript.md` under a `## <date> · sales call` heading, appended when the file already exists.

**The grade.** One table, PASS or FAIL, never a maybe, the evidence quoted in every row. `references/gates-and-rungs.md` carries the number behind each gate and what counts as a cost sentence; read it before you grade.

| Gate | Passes when |
|---|---|
| 1 LISTEN | The buyer talked more than the founder |
| 2 DIAGNOSE | 11 to 14 real questions, and the buyer said the cost of staying broken out loud |
| 3 ONE PRICE | One number, said plainly, then silence. No ranges |
| 4 NEXT STEP ON THE CALL | A date, a yes, or a clean no. Never "I'll send some info" |

Gate 2 fails one way above all: the founder started solving. Say it plainly.

Under the table: the one thing to do differently next call, quoting the moment. What they bought or refused, in their words. Where the deal stands, one of 4 words: closed · next step dated · stalled · dead. Then 2 or 3 ideas for this buyer only, each pointing at the line it came from.

Write `squad/clients/<first-last>/calls/<date>-debrief.md`: which input landed and whether it was rough, the gate table, those 4 parts. Append the buyer's verbatim lines to `squad/clients/<first-last>/notes.md` under `## QUOTES`, each labeled `(sales call · Marcus R · 2026-09-04)`: the cost sentence first, then what they already pay for, what they asked for that nobody sells, and the objection in their words.

**Then 3 writes into `squad/sales.md`, by exact heading string:**

- `## THE ONE FIX` is replaced, not appended: this call's one thing, one line.
- `## THE OBJECTIONS LEDGER` gains the objection in the buyer's words with the answer that moved it, or increments the count on one already there.
- `## THE CALL RECORD` gains one row: the date, the name, the 4 grades, where the deal stands, and in the last cell the previous call's one fix with whether it held.

No `squad/sales.md` yet: the debrief holds it all, and the update is parked in one line until the script runs.

**Stop only when the call argues with a line the founder confirmed** (the price, the promise, the warranty, the proof, a rung, a dated step, a spoken line). Print the line as it stands, the buyer's words that argue with it, and the change you propose, then wait for their yes. The price and the promise never move past what `squad/business.md` carries. 3 calls raising the same objection: say so in one line and send them to the Winning Offer, never before 3.

**The row.** Write it into `squad/pipeline.md`, 7 fields, the person's row rewritten in place when one exists, the header line first when the file is new, and print the row so they see what landed.

```
name · source · last bucket or outcome · date · next touch · what went out last · money
Marcus Reyes · warm, old agency client · interested · 2026-09-04 · 2026-09-08, partner call · call 2026-09-04, invite sent on it ·
Dane Okafor · inbound, "I Built a Cold Email Agent" · question · 2026-09-05 · 2026-09-09, bump · price question answered ·
```

The second field is how they came, then what brought them: `warm`, `cold` or `inbound`, then the founder's own words for a warm contact, the batch for a cold one, the piece an inbound reply named. A piece nobody named reads `inbound, source unknown`, and it stays that way.

The third field holds one of 7 values, never a sentence: `interested`, `question`, `objection`, `not now`, `no`, plus `signed, not paid` for a yes whose money has not cleared, plus `closed won` once it has. Next step dated is `interested`, a live price push is `objection`, stalled is `not now`, dead is `no`. For a call, "what went out last" is the call and what the founder sent on it. The money field stays blank until a payment clears, then it reads the amount and the date it cleared, `$997 cleared 2026-09-04`. **Signed plus paid is the only thing that makes a client.** Add the `pipeline` row to `.claude/squad-roots.md` when it carries none.

Never regrade a call whose debrief is on disk.

## Sort this reply · "sort this reply"

`references/reply-buckets.md` runs this mode: read it first. It carries the buckets, the moves, the next touches, the tiebreaks, the door, what every draft has to be, and the gate every draft passes before it prints.

Sort each reply into one of 5 buckets, the reason next to it in the founder's own terms so they can disagree: interested, question, objection, not now, no. A reply with no ask in it is not sales: a hello gets one real question back and no bucket.

No offer document is normal here. Put no number in any message, and answer a price question the honest way: it is not priced yet, so what would it be worth to them? Their answer goes to that folder's `notes.md` verbatim. A draft uses the script where one exists: its price line, its proof, any standing answer the ledger already proved.

A sender with no folder in `squad/clients/` and no row in `squad/pipeline.md` came off a piece, and the draft asks so: one line at the end, in the founder's own voice, "Where did you find me?" In the first draft back, or never.

Print the batch, interested and question first, then stop on one line: tell me what went out and I log it. The founder edits and sends by hand.

Then log. The pipeline row by the rule above. The buyer's verbatim lines to their folder's `notes.md`, labeled `(reply · Name · date)`; an objection also to `## THE OBJECTIONS LEDGER`, parked in one line when no script exists yet. Never create the script here. One bump, day 4, then nothing; nobody gets 2 messages in one day.

## Never

- Never send, never book, never charge, never write to any calendar, never upload a recording.
- Every number comes from `squad/business.md`. Never a price, a tier, a discount or a payment term the founder did not decide.
- Every promise and every warranty comes from the offer document, word for word in substance. Never a guarantee.
- The proof is the founder's own win, with how it happened. Never a claim you cannot source.
- Every quote is verbatim, labeled and dated. Never a paraphrase saved as a quote.
- Never invent the source, and never invent a day. A blank stays blank until they say it.
- One script. A second does not get read.
- Money means cleared. A booked call is not money, and a "let's do it" is not money.
