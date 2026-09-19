# ARKADIA: Ultimate Freshers Night

**One night · one Arkadia.** Organised by Utopia for SOAD & SOS.

**23 September · 6 PM – 12 AM** — freshers interaction by schools & reps, then a complimentary DJ night by Utopia.

**Pass: ₹500** via UPI (no gateway fees). Students register with student number (must start with `26`) + phone.

```
arkadia-website/
├── index.html            ← entire site + register/pay flow
├── AI_INSTRUCTIONS.md
├── README.md
└── assets/
```

## Before sharing with students

1. Open `index.html`, find `PAYMENT.upiId` near the bottom, set Utopia's UPI ID (example: `utopia@oksbi`).
2. Deploy / open the public GitHub Pages link.
3. Share that link in WhatsApp / Instagram.

## How payment works

- Student enters **student number** (must start with **26**) and **10-digit phone**.
- Site opens their UPI app (GPay / PhonePe / Paytm / BHIM) with **₹500** prefilled.
- Student number + phone go in the UPI note so Utopia can match payments.
- Money hits your UPI directly — **no Razorpay / gateway cut**.

## Local preview

Open `index.html` or run `python3 -m http.server 8080`.
