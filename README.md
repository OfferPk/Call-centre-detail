# Call Centre Detail — Offline App

Ek hi file ki offline app: Pakistan ke call centres / BPOs ki list — naam, phone,
location, campaign aur SECP registration status — bina internet ke Android phone
par check karein.

## Files

- `index.html` — poori app, data ke saath (single file, ~1.4 MB). Phone par
  download kar ke browser mein kholein — internet ki zaroorat nahi.

## Data (24 Nov 2026)

- **4,359** centres, **57** sheher
- SECP status: **270 registered**, **414 not registered**, 48 ambiguous,
  3,627 abhi check nahi hue
- Tier: **319 RED**, **19 YELLOW**, baqi normal (—)
- Islamabad: 552 centres — 343 SECP-checked (136 registered, 186 not registered)

## Card ke rang

- 🔴 **Laal — RED FLAG:** scam-pattern campaign ya SECP par register nahi
- 🟡 **Peela — YELLOW:** solar / energy campaign
- 🟢 **Hara — REGISTERED:** SECP par registered (CUIN ke saath)
- ⚪ **Grey — NOT CHECKED:** SECP status abhi check nahi hua

Note: SECP registration ka matlab "clean" nahi — agar campaign RED hai to
card laal hi rahega.

## Features

- Dashboard: total, registered, not registered, RED, Yellow, not checked, sheher
- Sheher ke hisaab se list (Islamabad, Rawalpindi, Lahore, Multan, Karachi…)
- Filters: City, Area, Tier, SECP status
- Search: naam, phone (0333 ya +92 dono chalte hain), location, status
- Card par tap karein to poori history: campaign/grounds, SECP notes, CUIN,
  website, Google Maps link; phone par tap kar ke direct call

## Rebuild

`~/workspace/nccia-poster/build_call_centres_app.py` — latest
`call-centres-registration-check-4359.xlsx` se `index.html` dobara banata hai.
