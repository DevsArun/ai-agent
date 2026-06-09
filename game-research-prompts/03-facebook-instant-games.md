============================================================
PROMPT: GAME TOPIC RESEARCH & VALIDATION (PHASE 1)
Platform: FACEBOOK INSTANT GAMES (Messenger + Facebook)  |  Target Geo: USA, Canada, Australia, UK (+ global)
Goal: Find ONE game concept with maximum SOCIAL-GRAPH virality + revenue potential
Targets: 100,000 plays in 20 days for this game; contributing to $3,000 / 20 days overall
Distribution: ORGANIC SOCIAL GRAPH (Messenger threads, friend challenges, leaderboards, group play). No ad spend.
============================================================

ROLE:
You are a senior Facebook Instant Games growth strategist + social-loop / virality analyst.
Your job is NOT to build yet. RESEARCH and RECOMMEND the single best game concept for FB
Instant Games, with data + sources.

CRITICAL PLATFORM CONTEXT (this is a SOCIAL-GRAPH platform — NOT search, NOT a feed):
- Distribution = the FRIEND NETWORK. Plays come from: messages shared into Messenger threads,
  "challenge a friend", custom update messages back to a thread, friend leaderboards, group
  play, and async turn-based PvP. The viral coefficient (K-factor) of the share loop IS the
  growth engine. Design the loop, not an SEO page or an FYP clip.
- HONEST RISK: Meta has deprioritized its gaming surface in recent years and there is
  permission-review / onboarding friction. The Instant Games tab is less prominent than it
  once was. Titles still launch here (e.g. established social/word titles), but a brand-new
  app with NO existing audience reaching 100k plays in 20 days requires an unusually strong
  native share loop AND passing app review in time. FLAG THIS UP FRONT.
- SDK = FBInstant: initializeAsync, setLoadingProgress, startGameAsync, getEntryPointData
  (so a challenged friend lands in the exact challenge), context.chooseAsync / createAsync /
  switchAsync (play inside a specific thread/group), updateAsync (post a custom challenge/score
  message back to the thread), shareAsync, getLeaderboardAsync (+ connected-player leaderboards),
  getInterstitialAdAsync, getRewardedVideoAsync, payments (IAP via FB).
- MONETIZATION: interstitial + rewarded video ads, and IAP via Facebook Payments. Tier-1 geo
  (US/CA/AU/UK) matters for eCPM. Async/competitive formats drive repeat sessions = more ads.
- BEST-FIT GENRES: social/competitive, word, trivia, quiz, async PvP, .io-style score battles,
  daily-challenge games, "beat your friend" hyper-casual — anything where beating/challenging a
  FRIEND is the core dopamine.

TEAM CONTEXT (do NOT reason as if this is a solo dev):
- The builder is a ~10-person full-stack TEAM (gameplay, art, sound, backend/netcode, growth/QA)
  running PARALLEL workstreams. The team CAN build async PvP, light real-time multiplayer, and
  richer social systems that a solo dev would avoid.
- DO NOT reject a concept for build effort alone — judge feasibility for a TEAM. The team's edge
  here is a tighter share loop AND more production polish than scrappy competitors. Reject only
  for strategic reasons (weak K-factor, app-review timeline, saturation).

DATA INTEGRITY & LIVE-VERIFICATION PROTOCOL (READ FIRST — mandatory, this is the #1 rule):
- BEFORE anything else, confirm you actually have LIVE web/research access THIS session and use it.
  * If you do NOT have live access, STOP and tell me plainly. DO NOT invent "live" citations and
    DO NOT present prior-knowledge guesses as verified facts. Either (a) ask me to paste the data,
    or (b) tag EVERY market claim "UNVERIFIED ESTIMATE — verify before building" and lower confidence.
- Every claim about a trending social format or competition MUST cite a source you actually opened
  THIS session (named URL), or be explicitly tagged as an estimate. No silent guessing.
- A concept whose advantage rests on an UNVERIFIED "thin competition / quality gap" claim MUST NOT
  become the final pick until that gap is verified against live competitors BY NAME (see STEP 1.5).
- Be brutally honest. No hype. Verified data beats confident guessing every time.

============================================================
STEP 0 — KILL TEST (do this BEFORE proposing anything)
============================================================
A) List 10 concrete reasons an FB Instant Game FAILS:
   e.g. share loop has K<1 so growth dies; no reason to challenge a friend; weak async/turn
   mechanic; app review blocks launch in time; depends on a big initial audience you don't have;
   not Messenger-thread-native; leaderboard not compelling; no daily reason to return; ad/IAP
   placement breaks the social flow; concept is single-player with no viral surface.
B) For EVERY candidate, run these 6 gates. Must SURVIVE ALL. Fail one -> REJECT + name it:
   1. SHARE-LOOP / K-FACTOR GATE — does playing NATURALLY create a message a friend will open + play?
   2. ASYNC-SOCIAL GATE          — is there a friend-vs-friend or thread/group hook (not just solo)?
   3. BUILD COMPLEXITY GATE      — can a ~10-person team ship a polished, mobile-first v1 within
      the sprint? (async PvP / light multiplayer is allowed; judge for a TEAM, not a solo dev)
   4. RETENTION GATE             — daily reason to return (challenge waiting, streak, leaderboard reset)?
   5. MONETIZATION GATE          — interstitial-at-transition + rewarded + optional IAP without killing the loop?
   6. ONBOARDING-TIMELINE GATE   — realistic to pass FB app review + start spreading inside 20 days?
C) Output a table: concept -> gates passed/failed -> verdict. Only ALL-pass survivors proceed.

============================================================
STEP 0.5 — REVENUE FEASIBILITY TEST (FB Instant model)
============================================================
For each survivor, show assumptions + math:
- Viral math: starting seed players * K-factor * cycle time -> can it reach ~5,000 plays/day
  (100k/20d)? Model K-factor honestly for a creator with NO existing audience.
- Revenue: interstitial impressions/session + rewarded acceptance % + IAP conversion %,
  realistic FB Instant eCPM for US/CA/AU/UK vs global mix.
- Sensitivity WORST | EXPECTED | BEST: K-factor, plays/day, projected 20-day revenue.
REJECT concepts that need a large seed audience you don't have. State plainly whether FB Instant
can realistically contribute to $3,000/20 days, or whether it's a long-shot social bet.

============================================================
STEP 0.75 — TEAM EXECUTION ADVANTAGE TEST
============================================================
Score 1-10 (this is a ~10-person team, NOT a solo dev):
- Can the team design a tighter, more human share loop AND out-polish funded social studios?
- Is the niche shippable by this team with a stronger K-factor than entrenched incumbents defend?
- Does the concept reward the team's ability to build real social systems (async PvP, leaderboards,
  challenge deep-links) rather than a loop any solo could clone?
Prefer 7+. Low score = a funded social studio will out-distribute you -> deprioritize.

============================================================
STEP 1 — TREND & DEMAND RESEARCH (social-graph native)
============================================================
Research and report with sources + approx numbers:
1. Which social/competitive web-game formats spread person-to-person in messaging right now
   (word, trivia, daily-puzzle, "beat my score", async PvP). Cite signals.
2. The mechanics of recent share-driven hits (e.g. daily-guess / streak / friend-challenge
   formats): what made people forward them into chats? Extract the transferable loop.
3. 5 games/mechanics that grew through friend challenges — for each, the EXACT message/moment
   that got forwarded.
4. What makes a challenge message irresistible to OPEN (curiosity gap, ego, streak protection).
5. Gap: which friend-challenge format is under-served specifically on FB Instant Games today.

============================================================
STEP 1.5 — OPPORTUNITY GAP ANALYSIS
============================================================
Score a table per format:
- Share-loop strength / expected K (High/Med/Low)   - Async-competitive fit (1-10)
- Daily-return strength (1-10)                        - # of strong incumbents on FB Instant (count + names)
- Build difficulty for the team (1-10)
PRIORITIZE: strong K-factor + strong async-competition + thin incumbent competition.
REJECT: formats dominated by entrenched social-game studios. Sort best-opportunity-first.

MANDATORY LIVE SATURATION CHECK (do this with real searches; name names — skipping this is failure):
- Separate broad social-format demand from SUB-NICHE saturation. A spreading format can already be
  owned by entrenched titles — that is the most common trap.
- For each candidate's EXACT mechanic + theme, search live (FB Instant Games listings + Google,
  e.g. "<mechanic> instant game", "<mechanic> messenger game") and LIST the real competitors BY
  NAME with URLs, count them, and judge their quality + how entrenched they are.
- If the specific sub-niche already has multiple established titles, mark it SATURATED and either
  REJECT it or require a concrete NOVEL differentiator (a real mechanic/share-loop twist — NOT
  merely "we'll have better polish").
- Cite the competitor URLs you actually opened. An unchecked "quality gap" claim is invalid.

============================================================
STEP 2 — CONCEPT SHORTLIST (propose 3, then pick 1)
============================================================
Only STEP 0/0.5/0.75 survivors. For each:
- Working title (memorable, "challenge me" friendly)
- One-line pitch (the social hook)
- Core loop (per round) + THE share/challenge loop (what message gets sent, why friend opens it)
- Why it's EASY to win early but compelling to keep challenging friends
- Build complexity (TEAM build within the sprint, mobile-first, Messenger-native; async PvP / light multiplayer OK)
- K-factor plan: exactly how each session generates new player invitations
- Daily-return plan: streaks, waiting challenges, leaderboard resets
- Monetization fit (interstitial at round-end, rewarded continue/hint, light IAP)
Then PICK THE WINNER and justify with the research data.

============================================================
STEP 3 — VALIDATE THE WINNER AGAINST THE 15 STRICT RULES (FB Instant lens)
============================================================
Explain CONCRETELY for EACH. If a rule can't be met, say so + fix.
1.  BOUNCE 0%: instant load via setLoadingProgress + startGameAsync, no real loading wall, small build.
2.  ABSOLUTE ADDICTION: dopamine loop in first 5s.
3.  EFFORTLESS PROGRESSION: easy early wins; player keeps beating the bar; time melts.
4.  PREMIUM MINIMALIST UI: clean, intuitive, mobile-first, thumb-reachable.
5.  TREND-ALIGNED METADATA: theme + mechanic match trending social/competitive formats.
6.  ORGANIC SHARE ENGINE: updateAsync / shareAsync / context loops that post challenges back to threads.
7.  SILICON VALLEY AESTHETIC: minimalist fonts, neon accents, kinetic transitions, juice.
8.  SELF-MARKETING LOGIC: challenge links, flex/shame cards, friend benchmarking via leaderboards.
9.  NATIVE SDK COMPLIANCE: full FBInstant SDK (context, updateAsync, leaderboards, getEntryPointData,
    interstitial + rewarded ads, payments) + all platform policies.
10. BULLETPROOF PRIVACY & POLICY: FB Platform policy + privacy/cookie compliance, minimal data, no PII misuse.
11. VIRAL EXPLOSION READY: a share loop engineered for K>=1 (each player brings >=1 more).
12. INVISIBLE AD PLACEMENT: interstitial only at round-end/transition; never mid-action.
13. MAX-YIELD REVENUE: rewarded triggers (revive/continue/hint/double) at high-intent moments + light IAP.
14. CREATOR BAIT: flex/result screens that look great when screenshotted into a chat or a clip.
15. LOW FRICTION = MAX REVENUE: easier = more rounds = more challenges sent = more sessions = more ads.

============================================================
STEP 4 — FINAL DELIVERABLE (output format)
============================================================
One-page "FB Instant Games Concept Brief":
- Final Title (+ 3 backups) + icon concept + the one-line challenge message template
- Genre + core mechanic (one paragraph)
- Social-format evidence (what's spreading in chats now; with sources)
- Team execution advantage score + revenue feasibility (worst/expected/best; ads + IAP)
- K-factor model (seed -> invites -> new players) + daily-return plan
- The EXACT challenge message + flex/shame card the loop sends, and why a friend opens it
- Monetization plan (where interstitial / rewarded / IAP fire without breaking the social flow)
- Why this beats existing FB Instant incumbents (the gap it fills)
- Risk/honesty note: app-review timeline + realistic K-factor for a no-audience solo dev in 20 days
- Build-spec handoff: screens, states, mobile-first layout, the ONE feeling +
  the ONE share moment the game must deliver.

CONSTRAINTS:
- Brutally honest, no hype. Prefer data + sources over opinion.
- Recommend ONLY ONE concept at the end.
- Any concept failing STEP 0/0.5/0.75 must NEVER reach the final pick.
- Flag UP FRONT if FB app-review / onboarding friction threatens the 20-day timeline, and
  recommend whether FB Instant should be a primary pillar or a parallel social bet.
- When (and only when) I reply "BUILD", proceed to Phase 2: implement the game with a UI
  measurably BETTER than the current top viral game in this niche on FB Instant, same core concept.
============================================================
