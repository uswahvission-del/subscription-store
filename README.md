# Nexa Digital Tools

Nexa Digital Tools website — production front-end baseline for digital subscriptions and direct WhatsApp ordering.

## Current catalog
- Ideogram Plus — 1 month — Rs 2,250 — 30 days complete warranty
- ChatGPT Plus — 1 month — Rs 3,250 — 25 days replacement warranty
- CapCut Pro — 1 month — Rs 550 — 27 days replacement warranty
- CapCut Pro — 6 months — Rs 3,500 — complete 6 months replacement warranty

### Ideogram reference
- Official reference price: $20/month on monthly billing + applicable tax
- Full private account
- Use on 3–4 devices easily

## Payment
- SadaPay — active
- JazzCash / Easypaisa / Binance USDT — shown as unavailable until account/payment details are finalized
- After payment, customer sends the payment screenshot on WhatsApp

## Contact
- WhatsApp ordering: +92 318 9836535
- Email: nexadigitaltools321@gmail.com
- WhatsApp community group and channel are linked from the website

## Production integration pending
- Secure admin authentication + dashboard
- Live orders/reviews/settings database
- Real AI assistant backend with multilingual responses
- Final production domain, canonical URLs, and live sitemap


## Current backend
- Orders are stored in the isolated `nexa_orders` table with Row Level Security.
- Customer submissions create a pending order and then open WhatsApp for payment confirmation.
- Reviews are stored as pending and appear publicly only after owner approval.
- Owner dashboard is private and requires an existing authorized Supabase admin account.
- Owner dashboard shortcut: `Ctrl + Shift + A` on desktop, or open the site with `#owner`.
- Active payment: SadaPay only.
- Sold counter remains hidden.
- The Nexa tables are isolated inside the currently connected Supabase project; they do not reuse the existing Uswah content tables.
- Supabase Free currently provides two active free projects; a separate Nexa project can be moved later if desired without changing the customer-facing flow.
