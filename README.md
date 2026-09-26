# FREQUENCY / Arkadia — archived portfolio project

**Status:** Event finished · **GitHub Pages disabled** · **No live payments**

Public repo for learning and portfolio: front-end event site, pass flow design, Razorpay + Google Sheets integration (removed from current source).

**Repo:** https://github.com/monish885-sys/utopia-arkadia

## What this was

Ultimate freshers night site for SOAD & SOS (23 September). Single-page HTML/CSS/JS with checkout and registration logging.

## What is turned off

| Item | Action |
| --- | --- |
| Public website | GitHub Pages **deleted** — old URL should 404 |
| Razorpay Key ID | **Removed** from `index.html` |
| Google Apps Script URL | **Removed** from `index.html` |
| Pass form | Replaced with “Sales closed” archive message |

## If you had a live Razorpay key in git history

Old commits may still contain a Key ID. In [Razorpay Dashboard](https://dashboard.razorpay.com/) → **Account & Settings → API Keys**, **regenerate or revoke** the key that was committed so it cannot be used even if someone finds it in history.

Also disable or delete the Google Apps Script web app deployment if you no longer need registrations.

## Run locally (preview only)

```bash
python3 -m http.server 8080
```

Open http://localhost:8080 — design and animations only; no checkout.

## Stack (for portfolio notes)

- Static site (no build step)
- Mobile-first UI, canvas disco backdrop
- Razorpay Checkout (was live during the event)
- Optional Google Sheets webhook for pass records
