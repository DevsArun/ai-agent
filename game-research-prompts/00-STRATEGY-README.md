# Multi-Platform Viral HTML5 Game Strategy — Master Briefing

> Goal: ship platform-specific, hyper-addictive HTML5 games that each clear **100k plays in 20 days** and collectively drive toward **$3,000 in 20 days**, using **organic distribution only** (no ad spend).
>
> One concept can be reused across platforms, but **graphics, pacing, and the distribution hook must be rebuilt per platform**, because each platform's discovery engine is completely different.

---

## 0. The single most important truth

These are **NOT** all "viral feed" platforms like TikTok. The thing that gives you 100k plays is a **different engine on every platform**. If you optimize for the wrong engine, you get zero traction no matter how good the game is.

| Platform | What actually drives plays (the "FYP equivalent") | Your job |
|---|---|---|
| **CrazyGames** | Platform recommendation algorithm (rewards D1 retention + playtime + CTR) **+ Google SEO** (crazygames pages rank for "X game online/free") | Win the 2-week **Basic Launch** metrics test so the algorithm graduates you to **Full Launch** and pushes you to the homepage |
| **Y8.com** | On-site category/related discovery **+ Google SEO** for "[game] y8". Audience is global & mixed-geo (lots of non-Tier-1) | Pick a high-search evergreen genre; rank and get auto-recommended |
| **Poki** | Poki's own enormous owned traffic — **Poki markets winning games for you** — gated behind a brutal quality/curation bar | Pass curation with top-1% polish + engagement-time metrics |
| **Facebook Instant Games** | The **social graph**: Messenger threads, group play, friend leaderboards, "challenge a friend", async PvP | Engineer share/challenge loops that ride the friend network |

**Takeaway:** CrazyGames + Y8 reward *search-friendly evergreen + retention*. Poki rewards *polish + curation*. FB Instant rewards *social virality*. The game concept can be shared; the **hook, metadata, and share mechanics cannot.**

---

## 1. Honest 20-day feasibility ranking (read before you build)

1. **CrazyGames — PRIMARY BET.** Self-serve, meritocratic algorithm, Tier-1 traffic (US/CA/AU/UK present), rewarded + midroll + banner ads at Full Launch. Realistic to hit big numbers fast if retention is good. Requires the game to be **not published on competing portals** for revenue share / exclusivity perks.
2. **Y8 — SECONDARY / EASY ENTRY.** Open upload (no approval wall). You monetize via **your own Google AdSense** + studio. Lower eCPM, mixed geo → revenue per play is lower; good for *volume + SEO*, weaker for pure dollars.
3. **Poki — HIGH CEILING, TIMELINE RISK.** If accepted, Poki's marketing can blow past 100k easily. But curation may not approve a brand-new solo dev inside 20 days. Treat as a parallel submission, not a guaranteed pillar.
4. **Facebook Instant Games — SOCIAL UPSIDE, ONBOARDING RISK.** Still live, but Meta has deprioritized gaming and there is permission-review friction. Great if your loop is genuinely social; risky as a revenue guarantee in 20 days.
5. **YouTube Playables — DEFERRED** (no account yet). Note: it **forbids external ad networks / payments** — Google controls monetization. Revisit after account approval.

> Brutal note: $3,000 in 20 days on **organic only** is aggressive. The math only closes if at least one game gets real algorithmic/SEO lift on CrazyGames or curation lift on Poki. Y8 alone will not get you there on dollars. Each prompt forces a worst/expected/best revenue model so you never fool yourself.

---

## 2. How to use these prompts

Each file in this folder is a **standalone Phase-1 prompt** for a single platform:

- `01-crazygames.md`
- `02-poki.md`
- `03-facebook-instant-games.md`
- `04-y8.md`

Workflow per platform:
1. Paste the platform's Phase-1 prompt into a strong reasoning AI **with web/research access**.
2. It runs the KILL TEST → revenue feasibility → solo-dev advantage → trend research → gap analysis → 3-concept shortlist → picks **ONE** winner with **data + sources** proving it's the best topic *for that platform*.
3. Only when you reply **"BUILD"** does it move to Phase 2 (implementation) — producing a game whose UI is **better than the current top viral game in that niche on that platform**, on the same core concept.

Run platforms **in feasibility order** (CrazyGames first). Reuse the winning core loop across platforms but re-skin + re-hook per the table above.

---

## 3. The 15 strict architectural rules (apply to EVERY build, every platform)

1. **BOUNCE RATE 0%** — load <2s, zero loading screen, canvas inits instantly.
2. **ABSOLUTE ADDICTION** — dopamine loop hooks within the first 5 seconds.
3. **EFFORTLESS PROGRESSION** — early levels easy; the player keeps winning and loses track of time.
4. **PREMIUM MINIMALIST UI** — dead simple, clean, intuitive; no clutter; thumb-reachable.
5. **TREND-ALIGNED METADATA** — theme + mechanic match the platform's highest-intent discovery signals (per-platform: SEO keywords / curation taste / social formats).
6. **ORGANIC SHARE ENGINE** — built-in loops that push players to share wins/fails through the platform-native channel.
7. **SILICON VALLEY AESTHETIC** — minimalist fonts, neon accents, smooth kinetic transitions, satisfying juice.
8. **SELF-MARKETING LOGIC** — challenge links, flex/shame cards, dynamic benchmarking baked in.
9. **NATIVE SDK COMPLIANCE** — fully implement the target platform's SDK + every developer guideline.
10. **BULLETPROOF PRIVACY & POLICY** — international privacy/cookie compliance, guest session tracking, no PII, age-appropriate (critical on kid-heavy Poki).
11. **VIRAL EXPLOSION READY** — a mechanic engineered to spawn endless shareable clips/moments.
12. **INVISIBLE AD PLACEMENT** — interstitials hidden inside level fade/transition; never mid-action.
13. **MAX-YIELD REVENUE** — high-intent rewarded triggers (rage-revive, continue, double, unlock) for max eCPM/yield.
14. **CREATOR BAIT** — record-perfect layout + "flex screens" creators naturally capture.
15. **LOW FRICTION = MAX REVENUE** — easier levels → longer play → more sessions → more ad impressions → more revenue.

---

## 4. Shared non-negotiables (so all builds stay portable)

- **Tech:** vanilla JS + Canvas (or one lightweight engine), self-contained build, no blocking external calls, instant init.
- **Size discipline:** keep initial load tiny (CrazyGames mobile-homepage eligibility needs ≤20MB; ≤50MB hard cap; FB/YT want small first loads). Build small from day one.
- **Abstraction layer:** wrap all SDK calls (ads, leaderboard, share, IAP) behind a single `Platform` adapter so the same core loop ports to each platform by swapping the adapter.
- **Analytics from minute one:** D1 retention, session length, ad-trigger acceptance, share-CTR. These metrics ARE the growth engine on CrazyGames/Poki.
