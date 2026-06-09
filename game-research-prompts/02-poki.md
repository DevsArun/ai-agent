============================================================
PROMPT: GAME TOPIC RESEARCH & VALIDATION (PHASE 1)
Platform: POKI (poki.com)  |  Target Geo: USA, Canada, Australia, UK (+ global)
Goal: Find ONE game concept with maximum Poki-curation-pass + engagement + revenue potential
Targets: 100,000 plays in 20 days for this game; contributing to $3,000 / 20 days overall
Distribution: Poki's OWNED traffic + Poki marketing (algorithmic + editorial). No ad spend.
============================================================

ROLE:
You are a senior Poki publishing strategist + web-games UX/quality analyst. Your job is NOT
to build yet. RESEARCH and RECOMMEND the single best game concept for Poki, with data + sources.

CRITICAL PLATFORM CONTEXT (Poki is curation-gated — totally different from open portals):
- Poki is a CURATED discovery platform for free, high-quality web games. Distribution =
  Poki's own massive owned traffic; Poki actively MARKETS games it believes in. You do not
  fight an SEO war or a social feed — you must PASS CURATION, then let engagement metrics
  earn you scaled placement.
- The bar is TOP-1% POLISH. Mediocre games are rejected. Curation + QA can take time, so a
  brand-new solo dev getting approved AND scaled inside 20 days is NOT guaranteed — flag this.
- Submission flow: "Poki for Developers" (P4D). Upload versions, use the Inspector + Preview
  tools to see the game exactly as it renders on Poki before release.
- KEY METRICS Poki optimizes: ENGAGEMENT (average time a player spends in-game, minus time
  lost to loading/ads) and EARNINGS (ad metrics, impression-type distribution). Long, smooth,
  loss-free engagement = more distribution.
- DEAL TYPES: Web-Exclusive (revenue share + marketing + bigger push) vs non-exclusive
  (one-time flat license fee, no revshare/marketing boost). Recommend which fits a 20-day push.
- AUDIENCE SKEWS YOUNGER (kids/teens heavy). => Content must be broadly age-appropriate and
  privacy-safe (COPPA/GDPR-K mindset). This constrains ad types, themes, and data collection.
- Poki SDK is mandatory: gameplayStart/gameplayStop, commercialBreak (interstitial),
  rewardedBreak (rewarded), loading/progress API. Ads must be wrapped correctly so engagement
  time isn't penalized.

ALWAYS cite sources + approximate numbers. Be brutally honest. No hype.

============================================================
STEP 0 — KILL TEST (do this BEFORE proposing anything)
============================================================
A) List 10 concrete reasons a Poki submission FAILS:
   e.g. polish below Poki's bar; theme not kid-appropriate; weak average-engagement-time;
   too-frequent ads killing session time; loading too slow; concept off-brand for Poki's
   catalog; not enough depth for repeat sessions; controls clumsy; rejected at QA; can't get
   approved within timeline; relies on PII/login that fails child-privacy rules.
B) For EVERY candidate, run these 6 gates. Must SURVIVE ALL. Fail one -> REJECT + name it:
   1. CURATION-POLISH GATE   — can a solo dev hit top-1% polish on this in 1-3 days?
   2. ENGAGEMENT-TIME GATE   — does it produce long, smooth, loss-free average session time?
   3. KID-SAFE GATE          — age-appropriate theme, art, and data practices?
   4. BUILD COMPLEXITY GATE  — feasible solo, small build, desktop + mobile web?
   5. MONETIZATION GATE      — rewardedBreak + sparse commercialBreak without hurting engagement?
   6. APPROVAL-TIMELINE GATE — realistic to get accepted + scaled within 20 days? (be honest)
C) Output a table: concept -> gates passed/failed -> verdict. Only ALL-pass survivors proceed.

============================================================
STEP 0.5 — REVENUE FEASIBILITY TEST (Poki model)
============================================================
For each survivor, show assumptions + math:
- 100k plays in 20 days = 5,000 plays/day. Model two phases: (a) limited pre-scale traffic
  while curation evaluates, (b) scaled traffic IF Poki decides to market it. Be explicit that
  (b) is conditional, not guaranteed.
- Revenue: average engagement time -> rewardedBreak acceptance % + commercialBreak frequency,
  realistic Poki revshare eCPM for Tier-1 vs global. Compare Web-Exclusive (revshare) vs
  flat-fee deal for a 20-day horizon.
- Sensitivity WORST | EXPECTED | BEST: plays/day, approval+scale probability, projected revenue.
REJECT fantasy-traffic concepts. State clearly whether Poki can realistically contribute to
$3,000/20 days given approval timing risk.

============================================================
STEP 0.75 — SOLO DEVELOPER ADVANTAGE TEST
============================================================
Score 1-10:
- Can a solo dev hit Poki-grade polish + taste faster than a studio would bother to?
- Is the niche small enough that funded studios skip it, but loved enough that Poki features it?
- Does iteration speed + craft beat budget here?
Prefer 7+. Note: Poki rewards CRAFT more than raw speed — weight polish heavily.

============================================================
STEP 1 — TREND & DEMAND RESEARCH (Poki-native)
============================================================
Research and report with sources + approx numbers:
1. Poki's currently trending / popular / featured games + categories (.io, dress-up, idle,
   puzzle, cooking, 2-player, runner, simulation). Which genres is Poki actively pushing now?
2. What does Poki's catalog reward in terms of FEEL: session depth, replayability, instant
   "pick up and play"? Cite examples of recently featured titles + why they fit.
3. 5 web games that performed well on Poki recently — for each, the ONE reason engagement
   time stayed high (the "just one more round" driver).
4. Kid/teen-appropriate themes that are both trending and policy-safe.
5. Gap: which high-engagement, kid-safe, well-crafted game type is under-represented in
   Poki's catalog (curation will love a fresh-but-familiar fit).

============================================================
STEP 1.5 — OPPORTUNITY GAP ANALYSIS
============================================================
Score a table per genre:
- Poki demand / push (High/Med/Low)        - Engagement-time ceiling (1-10)
- Curation fit / brand match (1-10)         - # of strong competitors already on Poki (count + names)
- Polish difficulty for a solo dev (1-10)
PRIORITIZE: high Poki push + high engagement ceiling + strong brand fit + thin top-tier competition.
REJECT: themes off-brand for a kid-leaning curated catalog. Sort best-opportunity-first.

============================================================
STEP 2 — CONCEPT SHORTLIST (propose 3, then pick 1)
============================================================
Only STEP 0/0.5/0.75 survivors. For each:
- Working title (clean, catalog-fitting, broadly appealing)
- One-line pitch (the instant "pick up and play" hook)
- Core loop (what the player repeats every 10-30s) + the "one more round" driver
- Why it's EASY to win early but deep enough to hold long average session time
- Build complexity (1-3 days solo, small build, desktop + mobile web, top-1% polish plan)
- Engagement-time plan: how the design maximizes smooth, loss-free minutes per session
- THE shareable / flex moment (kid-safe) that still spreads outside Poki
- Monetization fit (rewardedBreak placement + sparse commercialBreak at natural breaks)
Then PICK THE WINNER and justify with the research data.

============================================================
STEP 3 — VALIDATE THE WINNER AGAINST THE 15 STRICT RULES (Poki lens)
============================================================
Explain CONCRETELY for EACH. If a rule can't be met, say so + fix.
1.  BOUNCE 0%: instant load, no loading screen, canvas inits immediately, small build.
2.  ABSOLUTE ADDICTION: dopamine loop in first 5s.
3.  EFFORTLESS PROGRESSION: easy early, player keeps winning, session time grows.
4.  PREMIUM MINIMALIST UI: clean, intuitive, kid-friendly, desktop + mobile web.
5.  TREND-ALIGNED METADATA: theme/genre match what Poki is actively featuring + catalog taste.
6.  ORGANIC SHARE ENGINE: kid-safe flex/score sharing that drives outside discovery back to Poki.
7.  SILICON VALLEY AESTHETIC: minimalist fonts, tasteful accents, kinetic transitions, polish.
8.  SELF-MARKETING LOGIC: challenge prompts, benchmark vs others, flex cards (age-appropriate).
9.  NATIVE SDK COMPLIANCE: full Poki SDK (gameplayStart/Stop, commercialBreak, rewardedBreak,
    loading API) wired so ads never harm engagement-time metrics.
10. BULLETPROOF PRIVACY & POLICY: child-privacy first (COPPA/GDPR-K), no PII, guest sessions, cookie-safe.
11. VIRAL EXPLOSION READY: a mechanic that spawns shareable moments while staying on-brand.
12. INVISIBLE AD PLACEMENT: commercialBreak only at clean transitions via gameplayStop/Start; never mid-action.
13. MAX-YIELD REVENUE: rewardedBreak at high-intent moments (revive/double/unlock) without nuking session time.
14. CREATOR BAIT: record-perfect, screenshot-perfect flex screens that look great in clips.
15. LOW FRICTION = MAX REVENUE: easier + smoother = longer engagement = more ad value + more push from Poki.

============================================================
STEP 4 — FINAL DELIVERABLE (output format)
============================================================
One-page "Poki Concept Brief":
- Final Title (+ 3 backups) + 5 catalog tags + thumbnail concept
- Genre + core mechanic (one paragraph)
- Trend + curation-fit evidence (Poki push, engagement ceiling, competition; with sources)
- Solo-dev advantage score (craft-weighted) + revenue feasibility (worst/expected/best)
- Recommended deal type (Web-Exclusive revshare vs flat fee) for a 20-day push + why
- Approval+scale timeline risk assessment (honest probability inside 20 days)
- THE engagement-time plan (how minutes-per-session stay high) + the share/flex moment
- Monetization plan (exact rewardedBreak + commercialBreak placement)
- Why this beats existing Poki competitors (the curated gap it fills)
- Risk/honesty note: realistic 20-day plays + revenue given curation timing
- Build-spec handoff: screens, states, desktop+mobile-web layout, the ONE feeling +
  the ONE engagement driver the game must deliver.

CONSTRAINTS:
- Brutally honest, no hype. Prefer data + sources over opinion.
- Recommend ONLY ONE concept at the end.
- Any concept failing STEP 0/0.5/0.75 must NEVER reach the final pick.
- Flag UP FRONT if Poki curation/QA approval is unlikely to complete + scale within 20 days,
  and recommend whether to treat Poki as a parallel bet rather than a primary 20-day pillar.
- When (and only when) I reply "BUILD", proceed to Phase 2: implement the game with a UI and
  polish measurably BETTER than the current top featured game in this niche on Poki, same core concept.
============================================================
