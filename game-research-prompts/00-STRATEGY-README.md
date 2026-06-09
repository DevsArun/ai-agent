# Multi-Platform Viral HTML5 Game Strategy — Master Briefing

> Goal: ship platform-specific, hyper-addictive HTML5 games that each clear **100k plays in 20 days** and collectively drive toward **$3,000 in 20 days**, using **organic distribution only** (no ad spend).
>
> One concept can be reused across platforms, but **graphics, pacing, and the distribution hook must be rebuilt per platform**, because each platform's discovery engine is completely different.

---

## 0. Team & capacity (this changes the strategy)

This is **NOT a solo developer**. The team is **~10 people, full-stack**, capable of dedicated specialization (gameplay code, art/animation, sound/juice, backend/netcode, growth/SEO/QA) and **parallel workstreams**.

What that unlocks vs a solo dev — and the AI MUST factor this in:
- **Higher scope is on the table.** Mechanics a solo dev would reject purely for build effort — light multiplayer / `.io` netcode, richer 3D, deeper content, heavier art — are **feasible** and should NOT be auto-rejected for "too hard to build." Reject them only for *strategic* reasons (saturation, retention, monetization, timeline), never for "a solo dev can't."
- **Higher polish bar.** The team can hit top-1% production value → Poki curation becomes realistic, and CrazyGames thumbnails/feel can out-class incumbents.
- **PARALLEL MULTI-TITLE LAUNCH = the real fix for the money math.** 10 people can ship and launch **multiple titles across multiple platforms at once**. This directly defeats CrazyGames' ~14-day unmonetized Basic Launch blackout: stagger several titles so several are post-graduation (and FB/Y8, which monetize day-one) are earning simultaneously inside the 20-day window.
- **Honesty guard:** 10 people in 20 days is still **not** a 100-person studio — avoid true live-service/MMO scope, and remember more people ≠ more quality without coordination. Prefer ambitious-but-shippable.

---

## 0.1 The single most important truth

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
3. **Poki — HIGH CEILING, TIMELINE RISK.** If accepted, Poki's marketing can blow past 100k easily. With a 10-person team the **polish bar is reachable**, so the risk is *curation timing*, not build quality — approval may still not land inside 20 days. Treat as a parallel submission, not a guaranteed pillar.
4. **Facebook Instant Games — SOCIAL UPSIDE, ONBOARDING RISK.** Still live, but Meta has deprioritized gaming and there is permission-review friction. Great if your loop is genuinely social; risky as a revenue guarantee in 20 days.
5. **YouTube Playables — DEFERRED** (no account yet). Note: it **forbids external ad networks / payments** — Google controls monetization. Revisit after account approval.

> Brutal note: $3,000 in 20 days on **organic only** is aggressive even for a team. The single-title math is tight (CrazyGames blacks out monetization for ~14 days). The team's real edge is **parallel titles**: ship 3–5 games across CrazyGames + Y8 + FB simultaneously so several are earning at once, and the $3k becomes a portfolio number, not a single-game miracle. The math still only closes if at least one title gets real algorithmic/SEO lift (CrazyGames) or curation lift (Poki). Each prompt forces a worst/expected/best revenue model so you never fool yourself.

---

## 2. How to use these prompts

Each file in this folder is a **standalone Phase-1 prompt** for a single platform:

- `01-crazygames.md`
- `02-poki.md`
- `03-facebook-instant-games.md`
- `04-y8.md`

Workflow per platform:
1. Paste the platform's Phase-1 prompt into a strong reasoning AI **with web/research access**.
2. It runs the KILL TEST → revenue feasibility → team execution advantage → trend research → gap analysis → 3-concept shortlist → picks **ONE** winner with **data + sources** proving it's the best topic *for that platform*.
3. Only when you reply **"BUILD"** does it move to Phase 2 (implementation) — producing a game whose UI is **better than the current top viral game in that niche on that platform**, on the same core concept.

> ⚠️ **Data-integrity rule (baked into every prompt):** the AI must confirm it has **live web access** and verify all market claims against **named live competitors this session**. If it has no internet, it must say so and refuse to present guesses as facts. It must also separate **category demand** (e.g. "2 player games" is huge) from **sub-niche saturation** (e.g. the ragdoll-brawler sub-niche is already flooded with clones like Ragdoll Hit / Rooftop Snipers). A "thin competition" claim is invalid until verified — this prevents recommending a saturated niche on guesswork.

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
- **Size discipline (quality-first):** quality is the priority, NOT a tiny file size. Target an initial download **≤20MB** to stay eligible for the CrazyGames mobile homepage (the biggest traffic lever), and never exceed the **≤50MB hard cap**. Achieve the <2s feel via **progressive/smart asset loading** (load the first playable screen first, defer the rest) — not by stripping quality.
- **Abstraction layer:** wrap all SDK calls (ads, leaderboard, share, IAP) behind a single `Platform` adapter so the same core loop ports to each platform by swapping the adapter.
- **Analytics from minute one:** D1 retention, session length, ad-trigger acceptance, share-CTR. These metrics ARE the growth engine on CrazyGames/Poki.
