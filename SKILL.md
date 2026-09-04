---
name: the-close
description: Use this when money enters a conversation, by inbox or by call. The founder says "build my sales document", "run the Close", "/the-close script", "I just got off a call with [name]", "grade this call", "/the-close after", "update the script with this: ...", "sort this reply", "what do I say back", "continue the Close" (picking a stopped run back up), or pastes a reply, a DM, a whole inbox batch, a call transcript, or a recording path. It builds squad/sales.md, the one general sales script everything they say for money comes out of, from the offer document and 5 answers (the booking link, the payment link, the delivery days, the price line as they say it, one win and how it happened), renders the client-facing page from it, grades every call against 4 gates the moment it ends with the evidence quoted, files the debrief, writes what the call taught back into the script, logs the pipeline row, and sorts every reply into its bucket with a draft under it. When Google Drive is connected it puts the script in a Google Doc and prints the link. One script, sharper after every call. It never sends anything.
---

# The Close

The Winning Offer built the offer document. This skill sells it. **Your work, in one line:
build one general sales script, grade every call against 4 gates the moment it ends, and write
what the call taught back into the script.** The founder's part: 5 answers once, the call
itself, and their own hand on send.

You are the sales coach in the room, and coaches are specific: never "good job, tighten the
middle", always which gate failed, the line that failed it, the one thing to do differently.
**And you never send:** no email, no DM, no booking, no payment link, nothing written into any
calendar. You draft; their hand presses send.

**One file ranks above everything and it is not yours to invent.** `squad/business.md`, the
offer document, carries the promise, the warranty and **the price**. The founder's 5 answers
sit next to it (the booking link, the payment path, the delivery days, the way they say the
number, the one win they can name). Under those come the buyer's own words, from
`squad/clients/<first-last>/notes.md`, a thread or a transcript, and those beat anything you
write. You are last. No offer document means no price, and REPLY mode is the one entry that
runs without one.

This skill runs in ANY founder's repo. `.claude/squad-roots.md` is the per-repo instance file
every member-run skill reads first (founder name, product word, and the `clients`, `sales`,
`pipeline` and `script doc` rows where a run has written them), and its values win over the
`squad/` paths below, which are worked examples. A row reading "(none yet)" is an unanswered
field, not an override: the worked-example path stands until this run fills it. Legacy repos
carry `.claude/spine-roots.md`; read that when no squad-roots.md exists, and write
squad-roots.md when neither does. A founder with no brand name of their own means `<brand>` is
their own name. `<first-last>` is firstname-lastname, lowercased, the same folder the Winning
Offer's warm entry makes; `<date>` is the call's date, `YYYY-MM-DD`.

## The modes, and how they are called

| Mode | The founder says | Beats |
|---|---|---|
| script | "build my sales document", "run the Close", `/the-close script` | 0, 1, 2. Once; then updated in place after every call |
| after | "I just got off a call with [name]", "grade this call", `/the-close after`, a pasted transcript, a file path | 3, the moment the call ends |
| update | "update the script with this: ..." | 4, any time, with or without a call behind it |
| reply | "sort this reply", "what do I say back", a pasted batch | REPLY mode, the last section, off the map |

## The run map (where you run, where you STOP)

| Beat | Mode |
|---|---|
| 0 THE SOURCES | AUTO: the install check, the offer document, the recording paragraph said once |
| 1 THE SCRIPT | HUMAN INPUT: 5 answers, then AUTO build, then **STOP · GATE: the agenda line, the price line, whose win the proof is, the dated plan, the founder's yes**; then AUTO: the stamp, the roots row, and the Google Doc when a Drive connector answers |
| 2 THE PAGE | AUTO: rendered out of the script, printed |
| 3 AFTER | HUMAN INPUT: the transcript (a paste, a path, or a recording transcribed on the laptop), the notes, or nothing; then AUTO: the 4 gates with the evidence quoted, the debrief, the quotes, the script updated in place (**STOP · GATE only when a standing line would change**), the pipeline row, the two sheet cells as text |
| 4 UPDATE | HUMAN INPUT: the idea; then AUTO under beat 3's gate rule |

The beat numbers ARE the step numbers below. Never pause an automated beat to ask a small
question (batch it into the next gate); never run through a gate because the answer seems
obvious. A confirmed script means beats 0 to 2 are done: never rebuild it, never re-ask what it
answers.

**Resuming.** The rule keys on the OUTPUTS, never on a session's memory. Check them in this
order and continue at the first one missing or incomplete.

| Missing or incomplete | Resume at |
|---|---|
| `squad/sales.md` does not exist | beat 1 |
| `squad/sales.md` exists and its last line carries no `confirmed <date>` stamp | beat 1, THE GATE ONLY: never rebuild the script |
| the script is confirmed, the roots file has no `script doc` row, and a Drive connector answers | beat 1's Doc step only: the Doc, the link, the row |
| the script is confirmed and `squad/sales-page.md` does not exist | beat 2 |
| `squad/clients/*/transcript.md` carries a `## <date> · sales call` block with no matching `calls/<date>-debrief.md` | beat 3, the grade: read the call off that block, never ask for it again |
| a debrief exists and `## THE CALL RECORD` in `squad/sales.md` has no row for it | beat 3, the update |
| a debrief exists and `squad/pipeline.md` has no row for that person dated that call | beat 3, the row |

Never regrade a call whose debrief is on disk.

## The outputs (7 files, every run)

1. `squad/sales.md`: THE file, the general sales script. `references/sales-document.md`
   defines it section by section. Built once at beat 1, never per person, updated in place at
   beats 3 and 4.
2. `squad/sales-page.md`: the one client-facing page, rendered from the script at beat 2.
3. `squad/clients/<first-last>/transcript.md`: whatever beat 3 was given, saved as it came,
   appended under `## <date> · sales call` when the Winning Offer's warm entry already wrote one.
4. `squad/clients/<first-last>/notes.md`: beat 3 appends the call's verbatim quotes under
   `## QUOTES`, labeled and dated. The file the Winning Offer's warm entry made, when it
   exists; created with that one heading when this run makes the folder. The buyer's words
   live here and nowhere else.
5. `squad/clients/<first-last>/calls/<date>-debrief.md`: the 4 gates with their evidence, the
   one fix, the ideas, beat 3.
6. `squad/pipeline.md`: one row per person, 7 fields, the file with its header when it does
   not exist yet. The plan reads every row.
7. `.claude/squad-roots.md`: given the `sales`, `pipeline` and `script doc` rows in place. The
   `clients` row belongs to the Winning Offer's warm entry, never written here. Nothing else in
   it touched.

Nothing else gets written. Never `squad/calls/`, never `squad/offer-research.md`, never a
per-person sheet, never a pre-call file, never a follow-up draft, never a calendar event, never
the Outreach Sheet.

## Beat 0 · The sources

**The install check, before you spend any of the founder's input.** Three files inside THIS
skill's folder, next to `SKILL.md`, must open: `references/sales-document.md`,
`references/gates-and-rungs.md`, `references/reply-buckets.md`. Any missing: stop and say the
folder was downloaded without its `references/`, copy the whole skill folder in again. Buckets
or rungs guessed from memory are wrong quietly, which is the expensive way to be wrong.

**A fourth file, in another skill's folder, is read too when it is there:**
`the-winning-offer/references/recording.md`, the one home of the transcribe step. Missing means a
recording cannot be transcribed here: say so in one line and ask for a transcript instead (`.txt`,
`.md`, `.srt`, `.vtt`), then carry on. It never stops a run.

**Then read, and say in one line what opened:** `squad/business.md`, every
`squad/clients/*/notes.md`, and `squad/pipeline.md`.

**`squad/business.md` in one of three states:**

| The file | What it means here |
|---|---|
| last line carries `confirmed <date>` | the offer is forged: the price, the promise, the warranty, the refusals all come from it |
| exists, and its last line carries no `confirmed` stamp | enough to build the script. The price is its price line. The warranty and the refusals print `(none yet)` where blank. A price line marked `(proposed, not yet said out loud)` is the Winning Offer's stop, not this skill's: say the number out loud there. This skill never writes `squad/business.md` |
| does not exist | no price to say, no promise to make. Point at the Winning Offer and offer REPLY mode meanwhile, which puts no number in any message |

**The proof is the founder's own.** No proof file is read anywhere. Beat 1 asks for one win
and how it happened, and that answer, marked `(founder's own)`, is the receipt the pitch
carries. "None yet" is an answer, and it prints `(none yet)`.

**Recording, said once, the first time `script` runs.** Quoted from
`the-winning-offer/references/recording.md`, the one place it is written; run the install and
the transcribe step from there when a recording lands at beat 3.

> **A 60-minute sales call.** Record on Zoom from the desktop app and hand the file to your
> squad the same way; the transcriber takes an hour of audio in a few more minutes. Free Zoom
> ends every meeting at 40 minutes, one-on-one included, so a 60-minute call needs Zoom Pro,
> which also writes the transcript itself as a `.vtt` once cloud recording and the audio
> transcript are switched on, one time. No Zoom Pro: take the call on Cal Video or Google Meet
> and record it on the phone beside you, then hand that file over like any other.
>
> **Nothing recorded** means every quote is the founder's memory, labeled
> `(founder's recollection · Name · date)`.
>
> **File types.** Transcripts: `.txt`, `.md`, `.srt`, `.vtt`. Recordings: `.m4a`, `.mp3`,
> `.wav`, `.mp4`, `.mov`.

Never a bot in the meeting, never a meeting tool or a calendar connected to Claude, nothing
uploaded anywhere.

## Beat 1 · THE SCRIPT

Trigger: "build my sales document", "run the Close" before any call exists, `/the-close script`.
One general script, never one per person. The founder opens it with a buyer on the line and runs
it top to bottom.

**Ask 5 things, in one message, then build.** These 5 live nowhere on disk:

1. Their booking link, the URL where a stranger books an hour. None yet is an answer; cal.com's
   free plan with 60-minute slots on real hours is one way to get one.
2. Their payment link, as a URL or as the path a stranger would actually use.
3. What delivery looks like: day 1, when the first thing lands back, what is done by when.
4. The price line the way they will say it out loud, in their own words.
5. One win they can name, and how it happened. None yet is an answer.

Then read `references/sales-document.md` and write `squad/sales.md` in exactly that structure,
to its law (a heading per section, one-line paragraphs, the tables, the spoken lines in bold),
every section sourced the way that file says. Nothing in it that is not in the offer document
or those 5 answers.

**The order.** The guardrails first (the one fix, who I sell to, the refusals, the warranty,
the rungs), then the hour in the order it happens (the open, the 13 questions, the pitch, the
price, the ask, when they push, how the hour ends), then the accumulating half written empty,
each section reading `(none yet, no call logged)`, so beat 3 has a place to write.

**Words, not material.** Every section of the hour holds at least one bold sentence the founder
can read aloud. **The three rungs get decided here**, FULL, MIDDLE and FLOOR, out of
`references/gates-and-rungs.md`: what comes out if the number has to move, never the same thing
for less money. **The proof line** is answer 5, printed in the pitch with how it happened and
marked `(founder's own)`; "none yet" prints `(none yet)` and the pitch runs on 3 beats. **No
booking link yet:** write `[BOOKING LINK]`. **No payment link yet:** `[PAYMENT LINK]`. Both
flags print on the footer, and the page does not go out carrying either.

**Self-check before the stop.** Every heading present by exact string; every section of the
hour carrying a bold spoken line; no angle bracket surviving into a spoken line (a slot you
could not fill is filled now or turned into a square-bracket blank the buyer fills on the
call); no paragraph over 40 words.

**STOP · GATE.** Print the script whole, then stop on four lines, every one of them the
founder's and none answerable from disk:

- **The open's agenda sentence.** A sentence they would open with, promising no more than the
  offer document does.
- **The price line.** The number and the sentence they will say it in. You never adjust a price,
  never invent a tier, a discount or a payment term, never print one they did not confirm.
- **Whose win the proof is.** "Mine" is written as mine, and it is said as mine on the call.
- **The plan, in days or weeks, never phase names.** You never date a step they did not say.

Any line that fails gets rewritten and reprinted, that line only. On their yes, stamp the
script's last line `confirmed <today's date>`; that stamp is the only record the gate happened.
Then add the `sales` row to `.claude/squad-roots.md` if it carries none, no questions asked.

**Then the Google Doc, AUTO.** `## The Google Doc` in `references/sales-document.md` is the
whole procedure: the detection, the HTML with real headings and tables, the title "Sales script
· <founder name>", the link on one line, the `script doc` roots row. No connector: one line,
"connect Google Drive (g2) and I put it in Docs next time", and carry on. Never a second line,
never a retry.

## Beat 2 · THE PAGE

AUTO, out of the script, no new questions. Four sections, no fifth: **the promise** (one line,
in the buyer's situation), **the proof** (the pitch's win with how it happened; a proof reading
`(none yet)` leaves this section out and says nothing about it), **the plan** (the pitch's dated
steps), **the price** (the number, flat, what is included under it). Three of the four come out
of `## THE PITCH · minutes 40 to 50`, the fourth out of `## THE PRICE, AND THE SILENCE · minute
50`.

Write it to `squad/sales-page.md` and print it so they see what a buyer sees. **The booking
link is its only call to action**, and it has to be live before the page ships: a page still
carrying `[BOOKING LINK]` gets one line above it saying it does not go out until the link is
pasted in and reread. One page. It is rewritten when the offer document changes or when beat 3
changes a standing line, never on its own.

## Beat 3 · AFTER

Trigger: "I just got off a call with [name]", "grade this call", `/the-close after`, a pasted
transcript, a file path. Runs the moment the call ends, before anything cools.

### The read

On a resume, a `## <date> · sales call` block already in `transcript.md` IS what landed; grade off
it and skip the read.

Take, in this order, and say which one landed:

1. **Text:** a paste, or a path to `.txt`, `.md`, `.srt`, `.vtt`. Gates 1 and 2 graded by count:
   the two sides, the questions, the cost sentence. An app-written transcript (a Whisper export,
   a VTT) is marked rough in the debrief; its lines are quoted as they came and every quote off
   it carries ` · rough` in its label.
2. **The founder's notes:** gates 1 and 2 graded on their estimate, and the evidence cell says
   so. Two questions: roughly what share of the hour did they talk, how many questions did you
   ask. Every buyer line off the notes is labeled `(founder's recollection · Name · date)`.
3. **Nothing:** six questions. Those two, plus did they say the cost out loud and in what words,
   what number did you say, what did you agree to next, what did they push on.

A recording path (`.m4a`, `.mp3`, `.wav`, `.mp4`, `.mov`, Zoom's `audio*.m4a`) is transcribed on
the laptop, the same way the warm call is: one yes, once, to install the local transcriber, then
the text lands as rung 1 above. The install and the transcribe step are written once, in
`the-winning-offer/references/recording.md`; run them from there, and when beat 0 found no such
file, ask for a transcript instead. Nothing uploads. An install that fails gets one line,
MacWhisper (Mac) or Buzz (Windows), export `.txt`, hand it back, then wait.

Save what landed to `squad/clients/<first-last>/transcript.md`, labeled (transcript, rough
transcript, or founder's notes), always under a `## <date> · sales call` heading, appended when
the file already exists. That heading is what the resume rule reads, so it goes in every time.
Create the folder when it is new.

### The grade

Every call is graded against these 4 and nothing else. `references/gates-and-rungs.md`
carries the number behind each gate and what counts as a cost sentence when the cost was said in
time; read it before you grade.

| Gate | Passes when |
|---|---|
| 1 LISTEN | The buyer talked more than the founder |
| 2 DIAGNOSE | 11 to 14 real questions, and the buyer said the cost of staying broken out loud |
| 3 ONE PRICE | One number, said plainly, then silence. No ranges |
| 4 NEXT STEP ON THE CALL | A date, a yes, or a clean no. Never "I'll send some info" |

Grade them in one table, PASS or FAIL, never a maybe, each with its evidence quoted: the ratio
or the estimate and where the founder ran long, the question count and the cost sentence quoted
or "never said", the exact words used to say the number or "no number said", what was agreed
with its date or the line that dodged it. Gate 2 fails one way above all: the founder started
solving. Say it plainly.

Under the table, in this order:

1. **The one thing to do differently next call.** One, quoting the moment: "at minute 9 you
   answered a price question they had not asked; the answer was another cost question."
2. **What they bought or refused, in their words.** Verbatim, always.
3. **Where the deal stands:** closed · next step dated · stalled · dead. Nothing else rides
   inside those four words; the fix, the ideas and the objection each have their own home.
4. **IDEAS, two or three, for this buyer only,** each pointing at the line it came from: the one
   small thing to build or send next, what their own words say they would pay for next. Thin
   beats invented.
5. One line more, only when the decider question turned up somebody not on the call: who, and
   what they decide. The founder asks for the introduction, never a pitch aimed at a stranger.

### The file, and the quotes

Write `squad/clients/<first-last>/calls/<date>-debrief.md`: which input landed and whether it
was rough, the gate table with its evidence, the five parts above. Chat scrollback is not a
record; the resume rule reads this file.

Then append the buyer's verbatim lines to `squad/clients/<first-last>/notes.md` under
`## QUOTES`, each labeled `(sales call · Marcus R · 2026-09-04)`, ` · rough` added when the
transcript was: the cost sentence, what they already pay for, what they asked for that nobody
sells, the objection in their words. A call that raised no objection still writes its cost
sentence, usually the best line of the week. The Winning Offer compiles its buyer language from
these folders; nothing is written to `squad/offer-research.md` here.

### The script, updated in place

AUTO, in the same breath. This is the half that makes call six better than call one, and it
writes into `squad/sales.md` by exact heading string; `references/sales-document.md` owns what
each holds.

- `## THE ONE FIX` is replaced, not appended: this call's one thing, one line, at the top of
  the script.
- `## THE OBJECTIONS LEDGER` gains the objection in the buyer's words with the answer that moved
  it, or increments the count on one already there.
- `## WHEN THEY PUSH · minutes 50 to 60` gains a standing answer when a ledger row's answer
  worked on a real call: it replaces that objection's written line, marked `(worked on N
  calls)`. A standing answer that stops working loses its mark, and the ledger says what did
  not work after "Not:".
- `## WHAT BUYERS SAID` gains the cost sentence and the verbatim lines, each with its label.
- `## THE QUESTIONS I ASK · minutes 5 to 40` gets marked: a tick on a question that produced a
  cost sentence; a question nobody could answer twice replaced by the one the founder asked live
  that worked.
- `## THE CALL RECORD` gains one row: the date, the name, the 4 grades, where the deal stands,
  whether the previous call's one fix held.
- `## WHAT THE CALLS ARE ASKING FOR` gains the IDEAS, deduplicated; an idea three different buyers
  asked for gets marked.

**No `squad/sales.md` yet** (a first call that came off a reply): the debrief holds everything,
the quotes still go to `notes.md`, and the update is parked in one line until beat 1 runs.

**STOP · GATE, only when the call argues with a standing line:** the price, the promise, the
warranty, the proof, a rung, a dated step, or a spoken line (the agenda line, the ask line, an
answer already standing in WHEN THEY PUSH). Promoting an answer the founder's own call proved is
AUTO; changing a line the founder decided is not, and it waits for a yes. Print the line as it
stands, the buyer's words that argue with it, and the change you propose, then stop. The price
and the promise never move here beyond what `squad/business.md` carries. **Three calls raising
the same objection:** say so in one line and send them to the Winning Offer. The offer document
gets rewritten there, never here, and never before three.

### The row

Append the row to `squad/pipeline.md` in place, 7 fields, the header line first when the file
is new, and print the row so they see what landed:

```
name · source · last bucket or outcome · date · next touch · what went out last · money
Marcus Reyes · warm, old agency client · interested · 2026-09-04 · 2026-09-08, partner call · call 2026-09-04, invite sent on it ·
Priya Shah · cold, September list · closed won · 2026-09-04 · none · payment link, on the call · $997 cleared 2026-09-04
Dane Okafor · inbound, "I Built a Cold Email Agent" · question · 2026-09-05 · 2026-09-09, bump · price question answered ·
```

**The second field is the attribution, and it carries two parts: how they came, then the one
thing that brought them.** How they came is `warm`, `cold` or `inbound`. What brought them is
the founder's own words for a warm contact, the batch for a cold one, and for an inbound reply
it is **the piece**: the title of the video, post or page they name, copied off
`squad/content-log.md` when a row matches it. Ask for the piece once, inside the first draft
that goes back, one line, "Where did you find me?", never twice and never as a guess from
memory. Until they answer it reads `inbound, source unknown`, and it stays that way. That
field is the only place money is ever tied to a piece, which is why C6's Sunday read counts
money whose second part is missing as unattributed instead of assigning it.

The third field holds one of seven values, never a sentence: the five buckets from
`references/reply-buckets.md` (`interested`, `question`, `objection`, `not now`, `no`), plus
`signed, not paid` for a yes whose money has not cleared, plus `closed won` once it has. Next
step dated is `interested`, a live price push is `objection`, stalled is `not now`, dead is `no`.
For a call, "what went out last" is the call itself and what the founder sent on it (the invite,
the payment link), off the debrief. The money field stays blank until a payment clears.
**Signed plus paid is the only thing that makes a client.** Add the `pipeline` row to
`.claude/squad-roots.md` when it carries none.

Then hand back two cells as text, for the founder's own hand on the Warm tab of their Outreach
Sheet; the skill never opens the sheet:

- **Status:** `TALKING` while it is alive (a page that went out is still TALKING), `CLOSED` when
  it is finished either way, `NOT NOW` on a park.
- **Column 5, "What they said on the call":** part 2 of the debrief, verbatim.

## Beat 4 · UPDATE

Trigger: "update the script with this: ...", one idea in the founder's words, with or without a
call behind it. Do not re-run the map.

1. Find the section of `squad/sales.md` the idea belongs to. Print the line as it stands and the
   line you propose.
2. Apply it under beat 3's gate rule: AUTO in the accumulating half or a question's wording;
   **STOP · GATE** when it would change a spoken line, the price, the promise, the warranty, the
   proof, a rung or a dated step.
3. Log the idea under `## WHAT THE CALLS ARE ASKING FOR` with its source (the call, the reply, or
   "founder, <date>"), and count the buyers who asked for it.
4. At three buyers, one line: this is a signal, not a hunch; open the Winning Offer with the
   count. An idea that would change what is sold or what it costs never lands in the script at
   all: that is the Winning Offer's rewrite of `squad/business.md`, warm off your calls (g4) or
   cold off the market (g5), and the script copies it after.

## REPLY mode

Trigger: a reply lands and the founder pastes it, one or a batch, saying "sort this", "sort my
replies", "what do I say back". This is the hour before there is a call, in their own inbox.
**Warm or cold, every reply sorts here;** the pipeline row's `source` field carries which it was
and what brought them, by beat 3's rule.
Do not re-run the map: sort, draft, print, stop, then log what they say went out. Beat 0's
install check runs first, because this mode leans hardest on a reference file.

**What belongs here.** A reply with a door in it: a price question, "send me something", "can
we talk", an objection, a date. **A reply with no ask in it is not sales:** a hello or a catch-up
gets one real question back and stays where it came from. Answering a friendly hello with a next
step is the thing that reads as a bot.

**No offer document yet is normal here.** It gates a price, not an answer. Draft off
`squad/clients/<first-last>/notes.md` where the folder exists, put no number in any message, and
answer a price question the honest way: it is not priced yet, so what would it be worth to them?
Their answer goes to that folder's `notes.md` verbatim, labeled `(reply · Marcus R · 2026-09-04)`.

Five buckets, the reason written next to each in the founder's own terms so they can disagree:
interested, question, objection, not now, no. **`references/reply-buckets.md` runs this mode:**
what each bucket sounds like, the move, the next touch, the Status, the tiebreaks, which door the
interested ones get, what every draft has to be, and the gate every draft passes before it
prints. Read it before sorting a batch and again before printing one. A draft uses the script
where one exists: its price line, its proof, any standing answer the ledger already proved.

Print the batch on one screen, interested and question first because those decay fastest, then
**STOP.** The founder edits, sends by hand, and says what went out.

**A sender with no folder in `squad/clients/` and no row in `squad/pipeline.md` came off a
piece, and the draft asks so.** One line at the end of the reply, in the founder's own voice,
"Where did you find me?" That answer is the second half of the pipeline row's source field. Ask
it in the first draft back or not at all; a week later nobody remembers which video it was.

**Then log.** The pipeline row by beat 3's rule. The buyer's verbatim lines to their folder's
`notes.md`, labeled `(reply · Name · date)`; an objection also to `## THE OBJECTIONS LEDGER`,
same label, because an objection is evidence wherever it arrives. **No `squad/sales.md` yet:** the
objection stays in the buyer's `notes.md` and one line says it lands in the ledger the day beat 1
runs. Never create the script here. Then two cells as text for the
founder's hand on the Warm tab: the Status off the bucket's own row in
`references/reply-buckets.md`, never off judgment, and the next touch date. One bump, day 4,
then nothing; nobody gets two messages in one day. Last, one line for tonight's `/bip`: what
went out today and what it taught. A number goes in only when the founder said it, and money
means cleared: a booked call is not money, and a "let's do it" is not money.

## Rules

- Every message is scannable: a short header, then a table or short bullets. Grades go in
  tables. The founder is deciding, not studying.
- Every number comes from `squad/business.md`. Never invent a price, a tier, a discount or a
  payment term, and never print one the founder did not confirm at a gate.
- Every promise and every warranty comes from the offer document, word for word in substance.
  Never a guarantee it does not carry, never an outcome guarantee.
- The proof is the founder's own win, as they told it at beat 1, with how it happened. Never a
  claim you cannot source, never a win they did not name.
- Every quote is verbatim, labeled and dated. Never a paraphrase saved as a quote, never a name
  or a need the buyer did not give.
- Never invent the source. A piece the buyer did not name is not their source, and a blank
  second half stays blank until they say it.
- Every date in the plan comes from the founder's own delivery answer. Never invent a day.
- The buyer's own words beat anything you write. When their thread says it better, quote it.
- Grade honestly, with the evidence quoted. A FAIL they disagree with is a conversation; a PASS
  they did not earn is a deal they lose next month.
- One script, one page. A second of either does not get read.
- Never send, never book, never charge, never write to any calendar, never upload a recording,
  never open the Outreach Sheet.
