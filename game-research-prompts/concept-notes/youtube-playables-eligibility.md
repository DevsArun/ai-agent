# Concept Note — Can I apply to YouTube Playables with just a game link?

> Short answer: **No.** YouTube Playables is NOT a "submit a public game URL" portal (unlike Y8).
> It requires a built, self-contained game, a partner/developer account, the Playables SDK, passing
> a test suite, and Google-controlled monetization (no external ad networks or payments). A
> CrazyGames build cannot be reused as-is.

Live-verified this session. Date context: 2026.

---

## Why a link alone does not work

1. **The game must exist first.** HORDE RUSH is still a concept — there is no link yet. Build first.
2. **It's a portal upload, not a link submission.** You upload a **self-contained build** through
   Google's developer portal, integrate the **Playables SDK**, and pass the **SDK test suite**.
   Source: https://developers.google.com/youtube/gaming/playables
3. **Access is gated.** YouTube Playables is partner/application-based, not open self-serve like Y8.
   (User has no account yet — onboarding is a prerequisite and a timeline risk.)
4. **Monetization is Google-controlled — external ad networks & payment gateways are prohibited.**
   You cannot bring your own ad network, integrate external payment gateways, or link out to
   third-party storefronts. So a CrazyGames-SDK build's ads/IAP will NOT carry over.
   Source: https://playgama.com/blog/main/youtube-playables-monetization/

## Technical implication (matches our platform-adapter strategy)

- "Same link everywhere" is impossible — each platform needs its **own build + SDK adapter**.
- For YouTube Playables specifically, the CrazyGames version must be **re-built** with the
  Playables SDK and Google's monetization (interstitial/rewarded configured in the portal),
  with NO external ad/payment code.
- Build constraints: self-contained HTML5 (single package), zero external network calls,
  small first load (~30 MB cap noted in prior research), CSP headers applied when served on YouTube.

## Correct sequence for YouTube Playables

1. Build HORDE RUSH (CrazyGames version) first.
2. Obtain a YouTube Playables developer/partner account + approval.
3. Produce a **dedicated YT build**: Playables SDK, no external ads/payments (use Google's
   monetization), self-contained, within size limits.
4. Upload via the developer portal → pass the SDK test suite → review → live.

## Recommendation

Treat YouTube Playables as a **deferred, parallel port** (not a day-1 pillar):
- It cannot contribute to the 20-day target if the account/approval isn't in place.
- Prioritize CrazyGames (self-serve, fast) first; port to YouTube Playables once the core game is
  proven and the partner account is approved.
