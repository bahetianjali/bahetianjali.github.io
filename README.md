# America's Biggest Itches Nobody Is Scratching

### I read a news story. I couldn't stop thinking. So I started looking for the pattern.

---

A few days ago I read that Microsoft quietly cancelled thousands of AI coding licenses — not because the tools didn't work, but because they worked *too well*. Engineers used them constantly. The bill got out of hand. Uber burned through their entire 2026 AI tools budget in four months.

That stopped me cold.

We've been told AI is the great equalizer. The thing that lets a 3-person startup move like a 300-person company. But if Microsoft — with a $3 trillion market cap — can't sustain the cost of AI at scale, what does that mean for everyone else trying to build something?

I didn't have an answer. But I had a feeling this wasn't just an AI story. It felt like a symptom of something bigger.

---

## Then I remembered the J-Curve

I've been going through some masterclasses on startups and one concept kept coming back to me: **the J-Curve**. The idea that most startups don't fail because their idea is bad. They fail in the valley — the dip between early momentum and sustainable scale — where operational costs spike, complexity multiplies, and the margin between "this is working" and "we're burning out" collapses.

The Microsoft AI story is a perfect J-Curve moment. The tool worked. Adoption went up. Costs followed. The infrastructure wasn't ready for the scale.

And I started wondering: is this the same curve playing out across industries? Is there a pattern of problems — not just in AI, but in healthcare, immigration, SMB operations, enterprise tooling — where the gap between "this exists" and "this actually works at scale" is where companies go to die?

So I started looking.

---

## What I looked for — and how I scored it

I didn't want to just make a list of complaints. Anyone can do that. I wanted to find the problems that actually matter — the ones worth someone's life's work.

So I built a simple scoring framework. I call it a **Gap Score**. Three inputs:

- **TAM** (1–10): How big is the market if this gets solved?
- **Frequency** (1–10): How often is this problem actively complained about? (Reddit, HN, G2 reviews, Twitter — where people actually vent)
- **Whitespace** (1–10): How weak are existing solutions? Are there incumbents who technically solve this but leave massive friction?

**Gap Score = TAM + Frequency + Whitespace** (max 30)

Higher score = more urgent, more wide open, more worth building for.

Here's what I found across five areas.

---

## The 10 Gaps

---

### 🤖 AI Infrastructure — "The Cost Nobody Planned For"

**Gap 1: Enterprise AI Token Cost Management**

There's no "AWS Cost Explorer for AI." Companies are flying blind on what their AI usage actually costs until the invoice arrives. Microsoft, Uber, and Nvidia have all hit this wall publicly in the last 60 days. Internally, teams are calling it "tokenmaxx" — emergency token budgeting — but it's duct tape, not infrastructure.

| TAM | Frequency | Whitespace | **Gap Score** |
|-----|-----------|------------|---------------|
| 9   | 9         | 9          | **27/30**     |

*Who's trying:* Helicone, LangFuse — early, incomplete. No clear winner.

---

**Gap 2: AI ROI Measurement for Non-Technical Teams**

Every CFO is being asked: "Is this AI spend worth it?" Nobody has a clean answer. The tools that exist are either too technical (logs and dashboards for engineers) or too vague (anecdotal productivity reports). The layer in between — a business-language ROI layer for AI tools — doesn't exist in a mature form.

| TAM | Frequency | Whitespace | **Gap Score** |
|-----|-----------|------------|---------------|
| 8   | 8         | 8          | **24/30**     |

---

### 🏥 Healthcare — "The Paperwork That Kills People"

**Gap 3: Prior Authorization Automation**

Physicians spend an average of **13 hours per week** just on prior authorization paperwork. 70% of denials are eventually overturned and paid anyway — meaning most of that work is pure waste. A new CMS rule took effect January 2026 requiring faster decisions, but most health plans are still running on manual workflows and disconnected systems.

| TAM | Frequency | Whitespace | **Gap Score** |
|-----|-----------|------------|---------------|
| 9   | 9         | 7          | **25/30**     |

*Recent signal:* Coral just raised $12.5M (April 2026) to automate specialty provider back-office. The problem is confirmed real. The solution space is still wide open.

---

**Gap 4: Clinical Admin Staffing — The Invisible Bottleneck**

The most common reason a patient waits isn't clinical — it's administrative. Referrals stuck in fax queues. Discharge paperwork unprocessed. There's a growing shortage not of doctors, but of people to handle the administrative work around every appointment. AI can fill this gap, but the workflow integration layer is missing.

| TAM | Frequency | Whitespace | **Gap Score** |
|-----|-----------|------------|---------------|
| 8   | 8         | 7          | **23/30**     |

---

### 🏢 SMB Workflows — "Too Small for Enterprise, Too Complex for Spreadsheets"

**Gap 5: Metric Fragmentation in Small Teams**

Marketing, Sales, and Finance at a 50-person company each have their own version of "what's our revenue?" Half of every leadership meeting is spent arguing about whose numbers are right. The enterprise solution is a data warehouse and a BI team. SMBs can't afford either. The middle layer — lightweight metric alignment tools built for small teams — is thin.

| TAM | Frequency | Whitespace | **Gap Score** |
|-----|-----------|------------|---------------|
| 7   | 9         | 8          | **24/30**     |

---

**Gap 6: AI Integration for SMBs Without Technical Teams**

Big companies have AI task forces. SMBs have one person who "handles tech." The tools being built assume either no AI (legacy SMB software) or significant technical capacity (enterprise AI platforms). The 10–200 person company that wants to embed AI into their ops without hiring a data engineer has almost no good options.

| TAM | Frequency | Whitespace | **Gap Score** |
|-----|-----------|------------|---------------|
| 8   | 8         | 8          | **24/30**     |

---

### 🛂 Immigration & Admin — "A Broken System Running on Fear and Fax"

**Gap 7: Employer Immigration Compliance Tooling**

The H-1B fee just jumped to $100,000. ICE enforcement has become unpredictable. Immigration attorneys are fielding near-daily calls from panicked employers who don't know if they're compliant. Most mid-size companies manage this through spreadsheets and expensive outside counsel. The compliance layer between "we have international employees" and "we're definitely not in violation" is mostly manual.

| TAM | Frequency | Whitespace | **Gap Score** |
|-----|-----------|------------|---------------|
| 7   | 9         | 8          | **24/30**     |

*Recent signal:* Casium raised $5M seed (Oct 2025) to automate employer immigration case management. Validated problem, early market.

---

**Gap 8: Cross-Border Contractor Compliance**

Remote work opened the talent market globally. Companies routinely hire contractors in 15 countries without fully understanding the tax, legal, or misclassification risk in each. Existing tools (Deel, Rippling) cover big companies. The $5M–$50M revenue company hiring its first international contractors is dramatically underserved.

| TAM | Frequency | Whitespace | **Gap Score** |
|-----|-----------|------------|---------------|
| 7   | 8         | 7          | **22/30**     |

---

### 🔌 Enterprise Tooling — "Everything Talks, Nothing Connects"

**Gap 9: Procurement Data Fragmentation**

The average mid-size enterprise has procurement data in five or more disconnected systems. The result: no one can answer "what are we actually spending on vendors?" without a 2-week manual audit. There are expensive enterprise solutions (Coupa, SAP Ariba) but the mid-market — $50M–$500M companies — is dramatically underserved.

| TAM | Frequency | Whitespace | **Gap Score** |
|-----|-----------|------------|---------------|
| 8   | 7         | 8          | **23/30**     |

---

**Gap 10: Enterprise AI Governance — The "Who Approved This?" Problem**

Companies are deploying AI agents into real workflows without any visibility into what they're doing, what data they're touching, or who's accountable when something goes wrong. Audit trails, access controls, and approval workflows for AI actions don't exist in a standardized form. As AI moves from "assistant" to "agent," this becomes a liability problem.

| TAM | Frequency | Whitespace | **Gap Score** |
|-----|-----------|------------|---------------|
| 9   | 7         | 9          | **25/30**     |

---

## The Pattern I Found

Here's what surprised me: **the highest-scored gaps aren't about missing technology. They're about missing connective tissue.**

The AI tools exist. The healthcare mandate exists. The immigration system exists. What's broken is the layer that makes them usable at scale — the workflow integration, the cost visibility, the compliance guardrails, the metric alignment.

The J-Curve isn't killing companies because they built the wrong thing. It's killing them because the infrastructure around the right thing is fragmented, manual, and opaque.

And here's the other thing: most of these gaps share a core — they're all about **making something that exists for enterprises accessible to the companies that can't yet afford enterprise solutions.** The mid-market, the SMB, the 30-person startup that just hired its first international contractor.

That's the whitespace. That's where the next wave gets built.

---

## Where I'm Going With This

I'm not here to tell you I've figured this out. I haven't.

What I do know is that I find this genuinely interesting — the exercise of looking at the noise (Reddit threads, HN posts, G2 reviews, news headlines) and trying to find the signal underneath. The problems that are complained about constantly but solved poorly.

I want to keep doing this. More industries, more rigor, better scoring. And I'd love to build something that makes this kind of gap-mapping searchable and useful for founders — a place where you don't have to spend 40 hours on Reddit to find out what's actually broken.

If you're a founder who's living inside one of these gaps, or a researcher who thinks my scoring is wrong, or just someone who found this interesting — I'd genuinely love to hear from you.

This is just the start.

---

*What's an itch you can't stop scratching? Reply here or find me on LinkedIn.*
