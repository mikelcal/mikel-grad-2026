# Mikel Calderon — MIDS 2026 Graduation Site

Personal graduation invitation site for UC Berkeley MIDS Class of 2026.

## Pages

| File | URL | Purpose |
|---|---|---|
| `index.html` | `grad.mikelcal.co` | Main invitation + stats + timeline + force graph + library |
| `guestbook.html` | `grad.mikelcal.co/guestbook` | Firebase-powered guestbook |
| `privacy.html` | `grad.mikelcal.co/privacy` | Privacy policy |

## Deploy (GitHub Pages + custom subdomain)

1. Push to `main` branch
2. Repo Settings → Pages → Source: `main`, folder: `/ (root)`
3. Add `CNAME` record in your DNS:
   - Type: `CNAME`
   - Name: `grad`
   - Value: `your-username.github.io`
4. GitHub Pages will pick up the `CNAME` file automatically

## Firebase

Guestbook uses Firebase Realtime Database (`grad-guestbook` project).
Config is in `guestbook.html`. RTDB rules are in `rtdb-rules.json`.

**After deploying**, restrict your Firebase API key to `grad.mikelcal.co`:
Google Cloud Console → APIs & Services → Credentials → Edit API key → HTTP referrers

## Amazon Affiliate

Book links use tag `mikelcal-20`. Covers load via Open Library API (client-side, no auth needed).

## Built with

D3.js · Firebase RTDB · Open Library · devicons · IBM Plex + Playfair Display
Confetti: hand-rolled canvas · Force graph: clustered D3 simulation · Timeline: brushable D3

---
*± 200hrs margin of error · methodology: vibes + regression · Luna did not help*
