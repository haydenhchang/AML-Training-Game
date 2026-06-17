# Negative News — Sample Cases

Four fictional cases that pressure-test the "three judgments" mechanic (Same person? / Relevant? / Material & current?). Difficulty ramps across them. Every name, outlet, and event below is invented.

Hit-tagging legend the player uses:
- **DISMISS** — not a match, not relevant, or immaterial.
- **NOTE** — relevant but not decisive on its own (build-up).
- **MATERIAL** — true match + risk-relevant + material → drives escalation.

Dispositions: **CLEAR / EDD (enhanced due diligence) / ESCALATE (SAR) / REJECT.**

---

## Case 1 — "The Clean-Looking One" (Tutorial / Easy)

**Customer profile**
- Name: **Daniel R. Okafor**
- DOB: 1981-03-12 · Country: USA (Ohio) · Occupation: dentist, owns a small practice
- Account purpose: business operating account, ~$30k/mo deposits

**Search results (6 hits)**

| # | Headline | Source | Date | Subject details |
|---|---|---|---|---|
| 1 | "Local Dentist Daniel Okafor Wins Small Business Award" | Columbus Coastal Ledger | 2023-09 | Dr. Daniel Okafor, Columbus dentist |
| 2 | "Daniel Okafor, 19, Charged in Campus Vandalism" | Meridian Wire | 2014-04 | Daniel Okafor, age 19, student in Arizona |
| 3 | "Okafor Family Dental Opens Second Location" | Columbus Coastal Ledger | 2024-02 | Dr. Daniel R. Okafor |
| 4 | "Driver Cited After Minor Fender-Bender on Route 9" | Tribune Daily | 2022-06 | "D. Okafor," no other details |
| 5 | "Dentists Sue Insurer Over Reimbursement Rates" | Health Beat | 2023-01 | class action, 200+ dentists incl. Okafor practice |
| 6 | "Daniel Okafor Named to City Chamber of Commerce Board" | Columbus Coastal Ledger | 2024-05 | Dr. Daniel Okafor |

**Hidden truth:** Legitimate customer. No risk-relevant adverse media.

**Ideal tagging:**
- #1, #3, #6 → DISMISS (positive/neutral, but confirm same person — they corroborate identity).
- #2 → DISMISS — *wrong person* (age 19 in 2014 → born ~1995, not 1981; different state). Identifier mismatch.
- #4 → DISMISS — not risk-relevant (minor traffic) **and** unconfirmed match ("D. Okafor").
- #5 → DISMISS — civil dispute, dentist as *plaintiff*, not wrongdoing.

**Ideal disposition: CLEAR.**

**Teaching point:** Negative-sounding keywords ("charged," "sue," "cited") are not automatically adverse media. Check the match and the role first. *Lots of noise, zero signal* is a valid and common outcome.

---

## Case 2 — "The Common Name" (Medium · entity-resolution trap)

**Customer profile**
- Name: **John A. Martin**
- DOB: 1975-11-02 · Country: USA (Texas) · Occupation: freight logistics, owns Lone Star Freight LLC
- Account purpose: business account, high-volume cross-border payments to Mexico

**Search results (8 hits)**

| # | Headline | Source | Date | Subject details |
|---|---|---|---|---|
| 1 | "John Martin Sentenced to 8 Years for Wire Fraud" | Federal Docket News | 2025-02 | John P. Martin, 52, Florida investment advisor |
| 2 | "Lone Star Freight Expands Laredo Crossing Operations" | Texas Trade Journal | 2024-08 | John A. Martin, owner, El Paso |
| 3 | "Customs Seizes Shipment Linked to Border Freight Firm" | Meridian Wire | 2025-04 | unnamed "El Paso logistics company," DEA probe |
| 4 | "John Martin, Musician, Releases New Album" | Coastal Arts | 2024-11 | John Martin, UK, musician |
| 5 | "Trucking Exec John Martin Donates to Local Food Bank" | Texas Trade Journal | 2023-12 | John A. Martin, Lone Star Freight |
| 6 | "Three Charged in Cross-Border Cash Smuggling Ring" | Federal Docket News | 2025-05 | names withheld pending indictment; "Laredo-area freight operator" among them |
| 7 | "John Martin Pleads Guilty to DUI" | Tribune Daily | 2009-07 | John Martin, 41 at time, Ohio |
| 8 | "Lone Star Freight Named Mid-Size Employer of the Year" | Texas Trade Journal | 2022-05 | John A. Martin |

**Hidden truth:** *Suspicious — not yet proven.* The customer is very likely the unnamed operator in #3 and #6 (El Paso/Laredo freight, cross-border, matching footprint), but no hit names him outright. The "obvious" hit (#1, wire fraud) is a **wrong person**.

**Ideal tagging:**
- #1 → DISMISS — wrong person (John *P.* Martin, Florida investment advisor, not freight/Texas).
- #4, #7 → DISMISS — wrong person (musician UK; DUI Ohio 1975-born would be 34 in 2009, profile says 41).
- #2, #5, #8 → DISMISS/NOTE — true match, identity-confirming, not adverse.
- #3 → NOTE — risk-relevant (DEA, customs seizure) and matches the customer's *business footprint*, but not named. Material *as corroboration*.
- #6 → NOTE/MATERIAL — risk-relevant (cash smuggling), "Laredo-area freight operator" strongly fits; still unnamed.

**Ideal disposition: ESCALATE (or EDD at minimum).** Not because of the flashy wire-fraud hit — that's the wrong man — but because two unnamed-but-tightly-matching law-enforcement stories align with the customer's exact business and geography, against a high-risk activity (cross-border cash). The rationale must say: *dismissed #1 as non-match; escalated on the convergence of #3 + #6 with confirmed business footprint.*

**Teaching point:** The loudest hit is a decoy. Real risk here is *circumstantial convergence*, not a named conviction. Escalation can be correct on strong suspicion even without a named hit — that's literally what a SAR is for.

---

## Case 3 — "It Wasn't Him" (Medium-Hard · guilt-by-association trap)

**Customer profile**
- Name: **Priya Nair**
- DOB: 1988-06-21 · Country: Singapore · Occupation: co-founder, Halcyon Capital Partners (boutique advisory)
- Account purpose: personal wealth account, source of funds = company dividends

**Search results (7 hits)**

| # | Headline | Source | Date | Subject details |
|---|---|---|---|---|
| 1 | "Halcyon Capital Co-Founder Arvind Rao Arrested in Embezzlement Probe" | Asia Financial Wire | 2025-03 | Arvind Rao, the *other* co-founder |
| 2 | "Halcyon Capital Partners Under Regulatory Review" | Asia Financial Wire | 2025-03 | firm-level; mentions "co-founders Rao and Nair" |
| 3 | "Priya Nair Named Rising Star in Regional Advisory" | Coastal Business Monthly | 2022-10 | Priya Nair, Halcyon, Singapore |
| 4 | "Priya Nair Disputes Parking Fine in Viral Post" | Tribune Daily | 2021-08 | Priya Nair, Singapore |
| 5 | "Embezzlement Case: Rao Acted Alone, Co-Founder Cooperating, Say Prosecutors" | Asia Financial Wire | 2025-04 | prosecutors state Nair is a witness, not a suspect |
| 6 | "Priya Nair, Mumbai Actress, Cast in New Series" | Coastal Arts | 2024-09 | different Priya Nair, India, actress |
| 7 | "Halcyon Capital Freezes Operations Amid Probe" | Asia Financial Wire | 2025-04 | firm-level |

**Hidden truth:** *The customer is clean but proximate to serious financial crime.* Her business partner committed the crime; prosecutors explicitly cleared her (#5). But the firm is under review and her funds flow from it.

**Ideal tagging:**
- #1 → NOTE — risk-relevant and same firm, but the *subject is Rao*, not the customer. Not a match to her conduct.
- #2, #7 → NOTE — firm-level exposure; relevant context for *source of funds*, not personal wrongdoing.
- #3 → DISMISS — positive, identity-confirming.
- #4 → DISMISS — not risk-relevant.
- #5 → MATERIAL (exculpatory) — directly resolves her status: witness, cooperating, not a suspect.
- #6 → DISMISS — wrong person (actress, India).

**Ideal disposition: EDD, not Reject/Escalate-as-suspect.** She isn't the wrongdoer, but her wealth derives from a firm now frozen and under regulatory review — source-of-funds risk is real. Correct call: enhanced due diligence on source of funds + ongoing monitoring, **not** a SAR naming her as a suspect.

**Teaching point:** Adverse media about someone's *company or associate* is relevant context, not a verdict on the customer. And **exculpatory news counts** — #5 is one of the most important hits in the case. Over-escalating here (treating her as the criminal) is a scored *false positive*.

---

## Case 4 — "Buried on Page Four" (Hard · stale-news + reputation-laundering trap)

**Customer profile**
- Name: **Gregor Vance** (legal name Grzegorz Wancel, anglicized)
- DOB: 1969-01-30 · Country: dual UK / "Republic of Saint Aurel" (fictional high-risk jurisdiction)
- Occupation: founder, Vance Holdings (real estate + commodities)
- Account purpose: private banking, large initial deposit, source of wealth = "decades in commodities trading"

**Search results (page 1 of 4 shown first; deeper pages cost time)**

*Page 1 (free):*
| # | Headline | Source | Date | Subject details |
|---|---|---|---|---|
| 1 | "Philanthropist Gregor Vance Funds New Children's Hospital Wing" | The Coastal Ledger | 2025-01 | Gregor Vance, Vance Holdings |
| 2 | "Gregor Vance on Building a Commodities Empire (Sponsored)" | Business Vision (sponsored) | 2024-11 | promotional profile |
| 3 | "Vance Holdings Named Top Regional Investor" | Business Vision | 2024-06 | press-release style |
| 4 | "Gregor Vance Joins Opera Society Patrons' Circle" | Coastal Arts | 2023-12 | society page |

*Page 3 (costs time to load):*
| # | Headline | Source | Date | Subject details |
|---|---|---|---|---|
| 5 | "Saint Aurel Names Officials in Sanctions-Evasion Findings" | Global Sanctions Monitor | 2025-02 | lists "G. Wancel, commodities intermediary" |
| 6 | "Commodities Broker Grzegorz Wancel Fined in 2007 Sanctions-Busting Case" | Federal Docket News | 2007-09 | Grzegorz Wancel, sanctions evasion, fine + suspended sentence |

*Page 4 / foreign-language (costs time + translation):*
| # | Headline | Source | Date | Subject details |
|---|---|---|---|---|
| 7 | "[Translated] Wancel Linked to Front Companies in Saint Aurel Oil Trade" | Aurel Daily (translated) | 2025-03 | investigative piece naming Grzegorz Wancel |

**Hidden truth:** *Criminal / high-risk.* The customer's anglicized name hides a documented sanctions-evasion history and a current, named sanctions-evasion finding under his birth name, plus front-company allegations in a high-risk jurisdiction. Page 1 is a curated wall of philanthropy and sponsored content — reputation laundering.

**Ideal tagging:**
- #1, #4 → DISMISS — positive/neutral, identity-confirming only.
- #2, #3 → DISMISS — sponsored/PR, low evidentiary value (source-quality trap: looks like coverage, isn't).
- #5 → MATERIAL — current, credible, names "G. Wancel, commodities intermediary"; matches birth name + occupation + jurisdiction.
- #6 → MATERIAL — prior sanctions conviction under birth name; establishes pattern.
- #7 → MATERIAL — front-company allegations, named, current, in the customer's jurisdiction.

**Ideal disposition: REJECT / ESCALATE.** Sanctions-evasion nexus is near-disqualifying; at minimum SAR + decline. The rationale must connect **Gregor Vance ⇄ Grzegorz Wancel** (name change is the key to the whole case) and cite #5–#7.

**Teaching point:** Two compounding traps. (a) **Search depth** — the disqualifying evidence is on page 3–4 and behind a translation; an analyst who only reads page 1 (all PR) clears a sanctions evader. (b) **Name normalization** — screening only the anglicized legal name misses everything; you must screen the birth name / alias. Page 1 looking *too* clean is itself a signal.

---

## What These Cases Test (mechanic check)

| Case | Primary skill | The trap | "Fun" payoff |
|---|---|---|---|
| 1 Okafor | Relevance & match basics | Scary keywords, zero real risk | Confidence; learning to dismiss noise |
| 2 Martin | Entity resolution + convergence | Loud wrong-person decoy; real risk is unnamed | "The obvious hit was a decoy" |
| 3 Nair | Association vs. conduct; exculpatory news | Guilt by association; over-escalation temptation | Restraint rewarded |
| 4 Vance | Search depth + alias screening | PR wall on page 1; truth behind a name change & translation | "Page 1 was too clean" — digging pays off |

**Balance principle confirmed:** every case has plausible distractors that *look* like signal, the correct call is never "just trust the scariest headline," and at least one case (Nair) is scored as a loss for *over*-escalating — so the game punishes paranoia as well as laziness.
