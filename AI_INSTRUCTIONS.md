# Instructions for the AI assistant

> Paste this whole file (or upload it) **before** asking for changes. It tells the AI what the project is and which parts of the design must not drift.

## What this is
The website for **ARKADIA**, the **ultimate freshers night** organised by **Utopia** for **SOAD** and **SOS**.

| Fact | Detail |
| --- | --- |
| Date | **23 September only** |
| Time | **6 PM – 12 AM** |
| First part | From 6 PM, respective schools and reps conduct their **own freshers interaction** |
| Second part | Followed by a **complimentary DJ night by Utopia** |
| Audience | SOAD & SOS |

**Do not mention Day 1, Day 2, Free Fire, NGF Racing, or a multi-day fest.** This is one night only.

Taglines: "One night. One Arkadia.", "One night. One frequency.", "Enter Arkadia", "Ultimate Freshers Night".

**Never invent facts** such as prices, venues, prize pools or phone numbers. If something is missing, leave a visible placeholder and an HTML comment beginning with `TODO:`.

## Technical rules
1. **Keep it one file.** All CSS goes in the `<style>` tag and all JS in the `<script>` tag of `index.html`. No build step, no npm, no framework, unless the user explicitly asks to "scale up".
2. External resources are limited to **Google Fonts**. Images go in `assets/images/`, logos in `assets/logos/`, referenced by relative path.
3. **Mobile first.** Most visitors arrive from an Instagram bio link on a phone. Check every change at 375px wide: no horizontal scroll, and tap targets of at least 44px.
4. Respect `prefers-reduced-motion`.
5. Keep the semantic structure: one `<h1>` (the hero wordmark), `<h2>` per section, `alt` text on real images.

## Design system
### Colours (`:root`)
| Token | Value | Job |
| --- | --- | --- |
| `--bg` | `#07081a` | navy-black page background |
| `--cyan` | `#1fe4f2` | labels, secondary chips |
| `--magenta` | `#ff2ee6` | corner brackets, primary chips and buttons |
| `--lav` | `#f7d8fb` | headline fill |

Only two accent colours. Don't add greens, yellows or oranges.

### Fonts
| Variable | Font | Use |
| --- | --- | --- |
| `--f-wordmark` | Cinzel 900 | **only** the word ARKADIA (`.chrome`) |
| `--f-cond` | Barlow Condensed | headlines, chips, buttons, labels |
| `--f-wide` | Archivo wide 900 | "FREQUENCY" / "NIGHT" lettering |
| `--f-script` | Pinyon Script | handwritten accents |
| `--f-body` | Barlow | paragraphs |

### Components
`.chrome`, `.headline`, `.label`, `.rule2`, `.frame`, `.chips` / `.chip`, `.btn--primary` / `.btn--ghost`, `.phase`, `<canvas data-disco>`, `.reveal`

Tone: short, uppercase, poster-like.

## Open TODOs (search `TODO` in index.html)
- [ ] Set `PAYMENT.upiId` to Utopia's real UPI ID before sharing
- [ ] Real Utopia logo (`assets/logos/utopia.png`)
- [ ] Instagram, email and WhatsApp links in the footer
- [ ] `og:image` for link previews once the site is hosted

## Payments
- Pass is **₹500** via **UPI intent** (GPay / PhonePe / Paytm) — no gateway fees.
- Registration only collects **student number** (must start with `26`) and **phone**.
- Do not invent a UPI ID. Leave the setup banner until organisers paste theirs.

## Scaling up (only if asked)
For registrations, payments or an admin dashboard, convert to **Next.js (App Router)**. Keep tokens/classes as global CSS and split sections into components, then deploy on Vercel.
