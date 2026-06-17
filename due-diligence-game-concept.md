# Negative News — A Due Diligence Game

A single-player investigation game about **adverse media screening**: the analyst's craft of searching the open world for negative news on a customer, deciding which hits are *real, relevant, and material*, and reaching a defensible call. Where the existing **Know Your Customer** game is fast document-checking at a booth (Papers, Please style), this one is about **reading between the headlines.**

The core fantasy: *the search returns 47 articles about "John A. Martin." One of them is your guy, and he's not who he claimed to be. Find it before your shift ends.*

---

## 1. Premise

You are an adverse-media analyst at a bank. Each shift, customer names land in your queue. You run them through a (fictional) news/web search and get back a messy pile of articles, snippets, and database hits. Almost all of it is **noise** — wrong person, old news, irrelevant, or harmless. Buried in there may be the thing that matters: fraud charges, a corruption probe, a sanctions tie, a trafficking link.

Your job: separate **the signal from the noise**, decide whether the negative news is *true-match, relevant, and material*, and disposition the customer — **Clear / Flag for EDD / Escalate (SAR) / Reject** — with a rationale that would survive an audit.

---

## 2. Core Loop

```
Receive name  ->  Run search  ->  Sift hits (match? relevant? material?)
     ^                                          |
     |                                          v
 Next case  <-  Consequences  <-  Disposition + write rationale
```

1. **Receive** a customer name + minimal profile (DOB, country, occupation, business).
2. **Search** — a results list appears: headlines, sources, dates, snippets.
3. **Sift** — open hits, judge each on three axes (below), tag them, take notes.
4. **Disposition** — Clear, Flag for EDD, Escalate, or Reject — and cite your evidence.
5. **Consequences** — resolve over later shifts; missed true hits and false alarms both cost you.

---

## 3. The Three Judgments (the heart of it)

Every article hit must be assessed on three questions. This is the real skill of adverse media screening, turned into the game's core verbs:

1. **Is it the same person? (Entity resolution)**
   - Match the article's subject to your customer using identifiers: full name, DOB, location, employer, photo, middle initial, age.
   - Traps: common names, "John A. Martin" vs "John Anthony Martin," same name different country, a relative with the same name, a deliberately similar alias.

2. **Is it relevant? (Risk relevance)**
   - A speeding ticket ≠ a money-laundering indictment. Categorize the news: financial crime, corruption, fraud, violent crime, terrorism/trafficking, regulatory action, civil dispute, or *not risk-relevant at all*.

3. **Is it material & current? (Materiality)**
   - How serious, how credible the source, how recent, charged vs. convicted vs. acquitted vs. merely *alleged*?
   - A 1998 dropped charge from a tabloid weighs differently than a 2025 DOJ indictment from a wire service.

**Only a hit that is all three — true match, risk-relevant, and material — should drive an escalation.** The game's difficulty is that the noise is designed to *look* like signal.

---

## 4. What the Noise Looks Like (the design challenge)

A good case buries 0–3 real hits in a pile of plausible distractors:

- **Wrong-person hits** — same name, different DOB / city / industry.
- **Stale news** — real but 20 years old and resolved.
- **Soft news** — a lawsuit over a fence line; a parking fine; a divorce.
- **Source-quality traps** — a sensational blog vs. Reuters; an anonymous forum post.
- **Guilt-by-association** — the customer's *cousin* / former business partner is the criminal, not them.
- **Reputation laundering** — a press release burying old fraud; SEO pushing bad news to page 4.
- **The real thing** — sometimes subtle: a small-print regulatory settlement, a foreign-language source, a name spelled slightly differently.

---

## 5. Tension & Constraints

- **Time per shift** — a full queue you can't read end-to-end forces triage. Skim or deep-read?
- **Search depth costs time** — page 1 is free; "load more," translate a foreign source, or pull the full article each cost time you may not have.
- **Two failure modes (asymmetric):**
  - *False negative* — you cleared someone with a real, material hit → fine, regulatory finding, story beat.
  - *False positive* — you escalated a wrong-person / irrelevant hit → wasted compliance resources, angry legit customer, "the business" complains.
- **Pressure from above** — clear the queue faster; a "VIP" client wants a clean bill. Do you read carefully or rubber-stamp?

The best players aren't the most suspicious — they're the most **calibrated**.

---

## 6. Scoring & Progression

- **Per-case grade** — correct disposition + correct hit tagging (did you catch the true match and dismiss the noise correctly?) + efficiency.
- **Defensibility** — the headline metric: a documented rationale ("dismissed hit #3: DOB mismatch; escalated hit #5: 2025 wire-service fraud indictment, identity confirmed via employer") scores well even if the final truth surprises you. Models real audit review.
- **Career arc / unlocks** — start with clear-cut single-hit cases → common-name nightmares → foreign-language sources → entity networks (the bad actor is hidden one hop away) → corporate adverse media (the *company's* directors, not the person).
- **Meta-events** — a regulator audits a sample of past calls; a news story breaks about someone you cleared.

---

## 7. Modes

- **Career / Campaign** — progression above, with a light thread: a recurring name keeps surfacing across cases, hinting at a network you slowly piece together.
- **Daily Case** — one hand-crafted name per day, shareable score.
- **Time Attack** — max accurate dispositions against the clock.
- **Training / Tutorial** — guided cases teaching the three judgments one at a time.

---

## 8. Tone & Aesthetic

Consistent with the existing **Know Your Customer** game: retro-terminal / grimy bureaucratic desk (VT323 / Special Elite fonts, aged paper, stamp interactions). The signature screen here is a **search-results feed** — a scrollable list of fake headlines you click to expand — plus a **dossier panel** where you drag hits into *Dismissed / Relevant / Material* buckets, and a final **sign-off stamp** (CLEAR / EDD / ESCALATE / REJECT).

---

## 9. Why It Works

- **Replayable** — procedural cases assembled from a library of real-feeling headlines + identifier traps.
- **Teachable** — every verb maps to a real adverse-media concept (entity resolution, relevance, materiality, source quality), so it doubles as analyst training.
- **Tense** — finite time + asymmetric failure costs make every "dismiss or dig?" a real decision.
- **Satisfying** — the payoff when the one article that didn't fit cracks the case.

---

## 10. Locked Decisions

- **Standalone game.** Not a mode inside the existing KYC game. Its own entry point, its own progression. (May still *reuse* the visual engine — see open questions.)
- **Fully fictional, always.** Every customer, name, company, headline, and source is invented. No real people, real companies, or real news — ever. This is a hard rule, not a preference: it keeps the game safe to ship and removes any defamation / privacy risk. Names should be generated to feel plausible but be clearly synthetic (e.g. drawn from a fictional-name generator, fictional outlets like "Meridian Wire" / "The Coastal Ledger").

## 12. Making It Fun (the juice)

The risk with the design above is that it reads as a *sorting task* — open hits, judge, drag to a bucket. Correct, but passive. These mechanics turn the analyst's craft into something you *do* with your hands, *feel* in your gut, and get *surprised* by.

### 12.1 Active search, not a static list
The search bar is the primary toy. You don't receive a list — you **build the query**.
- Start with a name and get 200 garbage hits. The game is *narrowing*: add `+DOB`, `+"Meridian Capital"`, `-football` (the other John Martin is a striker), quote an exact phrase, or restrict to a date range.
- Each refinement is a small puzzle with a tactile payoff: the feed visibly collapses from 200 → 40 → 6. Watching the noise melt away is the loop's core dopamine.
- **Over-narrowing is a trap** — too many filters and you'll filter *out* the one real hit (it used a middle initial you excluded). Calibration applies to the search itself.

### 12.2 The corkboard (the detective fantasy)
A second screen: a **cork pinboard with red string**. Drag entities — people, companies, addresses, the customer — onto the board and physically draw connections.
- The "bad actor is one hop away" cases (§6) become *spatial*: you pin the cousin, the shell company, the shared address, and the line you draw between them is the insight.
- Snapping a connection that resolves the case triggers the signature **"it clicks"** moment — the string pulls taut, the linked nodes pulse, a stamp slides into reach.
- This is where humor and dead ends live too: pin three things that *look* connected, find no string fits, and you've learned it's a coincidence.

### 12.3 Make the consequences have faces
Numbers don't sting. People do. Borrow Papers, Please's emotional hooks:
- **The cleared man on the evening news.** Three shifts after you clear someone, a chyron crawls across your monitor: *"MERIDIAN EXEC ARRESTED — laundering ring."* It's the guy. The memo from your boss lands the next morning. You *remember* his case.
- **The angry legit customer.** Over-escalate a wrong-person hit and a furious email arrives: a small-business owner whose accounts you froze over his criminal namesake. Now you feel the false-positive cost.
- **Recurring NPCs with voice:** a smarmy Relationship Manager who leans on you to fast-track his VIP ("she's a *philanthropist*, just clear it"); a deadpan auditor who samples your old calls; an anonymous tipster who DMs you a half-redacted lead — trustworthy or a setup?

### 12.4 Risk/reward on the clock (gambling with time)
Make "skim or dig?" a *bet*, not a chore.
- **Dig actions cost time and may pay nothing.** Translate the foreign-language source (90 sec) — it's either the smoking gun or a recipe blog. Pull the full archive — paywall, dead end. The tension is real because the cost is real.
- **Calibration streak / combo.** Consecutive correct dispositions build a "Sharp" multiplier that boosts score *and* buys back time. Break it with a sloppy rubber-stamp and you lose the streak — discouraging the very laziness the job punishes.
- **The hot-streak temptation:** the higher your streak, the more the game dangles an easy-looking clear to make you drop your guard. The VIP case always arrives when you're cocky.

### 12.5 Juice & feedback
Every interaction should feel good in the hand.
- The **sign-off stamp** has weight: a satisfying *cha-chunk*, ink bleed, the dossier slamming into the OUT tray.
- The feed's distractors include **deadpan-funny filler** for tonal relief: *"Local Man Wins Regional Chili Cook-Off Third Year Running,"* *"J. Martin's Fantasy Football League Erupts in Scandal."* Levity makes the real hits hit harder.
- **The reveal.** When a case resolves, a short "what was actually true" beat plays — sometimes vindicating, sometimes a gut-punch twist. This is the payoff §9 promises; give it a real animation moment.

### 12.6 Twists & set-piece cases
Procedural cases are the bread; **hand-crafted twist cases** are the dessert that gets talked about.
- **The obvious villain who's innocent** — every signal screams guilty; it's a wrong-person trap, and escalating tanks you.
- **The boring clear who isn't** — a textbook clean profile with one foreign-language footnote that cracks everything.
- **The call from inside the house** — the customer is your own bank's executive, and your boss *really* wants this one cleared.
- **The slow-burn network** (campaign): one recurring synthetic name surfaces across unrelated cases for weeks until the corkboard finally reveals the web. The campaign's spine.

### 12.7 Difficulty as escalating *feel*, not just harder traps
Early shifts: roomy clock, clear-cut single hits, the tutorial NPC at your elbow. Late shifts: the queue is brutal, the clock is mean, two screens are blinking, the RM is emailing you, and an audit is mid-sample. Fun here is the **overwhelm-then-master** arc — week one you're drowning, week six you're slinging filters and snapping red string like a pro.

---

## 11. Still Open (decide before building)

1. **Case authoring** — hand-crafted headline sets (higher quality) vs. procedural generation from a snippet/identifier library (replayable)? Hybrid is likely best.
2. **Realism dial** — pure entertainment vs. genuine analyst-training tool? Changes how forgiving scoring is and how detailed the headlines must be.
3. **Session length** — quick 5-minute daily vs. longer 15–20 min deep-read sessions?
4. **Visuals** — reuse the existing pixel/terminal engine, or build a dedicated search-feed + dossier UI?
