# ARKADIA — Pass · ₹500

Organised by Utopia for SOAD & SOS · **23 September · 6 PM – 12 AM**

**Public link:** https://monish885-sys.github.io/utopia-arkadia/

## Can personal UPI take 400 × ₹500?

**No.** Personal UPI usually caps around ~20 credits/day. 400 passes need a **merchant checkout**.

Use **Razorpay** (free to open, KYC once). It accepts UPI / cards / net banking at any volume. Standard fee is about **2% (~₹10 per pass)** — that fee is what makes 400 payments possible.

## Setup (5 minutes)

1. Sign up at [razorpay.com](https://razorpay.com) → complete KYC → activate Live mode.
2. **Account & Settings → API Keys → Generate Key** → copy **Key ID** (`rzp_live_…`).
3. Open `index.html`, find `PAYMENT.keyId`, paste the Key ID.
4. (Optional backup) Create a **Payment Link** for ₹500 → paste into `PAYMENT.paymentLink`.
5. Push / redeploy so students get the update.

```js
const PAYMENT = {
  amountInr: 500,
  keyId: 'rzp_live_xxxxxxxx',   // required
  paymentLink: '',              // optional backup URL
};
```

Never put the **Key Secret** in this file.

## Student flow

1. Opens the site on phone → **Pass · ₹500**
2. Enters **student number** (must start with `26`) + **phone**
3. Razorpay checkout opens → pays ₹500
4. Site shows **Pass Secured** with payment ID (also in Razorpay dashboard notes)

## Deploy

Repo: https://github.com/monish885-sys/utopia-arkadia  
Pages: https://monish885-sys.github.io/utopia-arkadia/
