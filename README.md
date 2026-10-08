# Nexa Digital Tools

Nexa Digital Tools website — production front-end for digital subscriptions, local payment and direct WhatsApp ordering.

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
- SadaPay number: 03116484535
- Account title: ABDUL REHMAN
- After payment, customer sends the payment screenshot on WhatsApp
- JazzCash / Easypaisa / Binance USDT are currently unavailable

## Contact
- WhatsApp ordering: +92 318 9836535
- Email: nexadigitaltools321@gmail.com
- WhatsApp community group and channel are linked from the website

## Completed production work
- Supabase-backed order persistence with Row Level Security
- Customer order tracking by Order ID
- Owner dashboard with authorized Supabase login
- Order status management
- Review submission with owner approval workflow
- Public approved reviews
- SadaPay copy-to-clipboard flow
- Live product search with keyboard navigation
- Vercel production deployment
- Production robots.txt and sitemap.xml

## Remaining production work
- Add the final custom domain when it is purchased/connected
- Complete Google Search Console submission and indexing checks
- Real AI assistant frontend/backend wiring is deployed; add the `GEMINI_API_KEY` Supabase Edge Function secret to activate live Gemini replies
- Owner admin email is verified in Supabase and password recovery is wired; final sign-in test requires the owner to set/enter the password

## Current backend
- Orders are stored in the isolated `nexa_orders` table with Row Level Security.
- Customer submissions create a pending order and then open WhatsApp for payment confirmation.
- Reviews are stored as pending and appear publicly only after owner approval.
- Owner dashboard is private and requires an authorized Supabase admin account.
- Owner dashboard shortcut: `Ctrl + Shift + A` on desktop, or open the site with `#owner`.
- Sold counter remains hidden.
- The Nexa tables are isolated inside the connected Supabase project; they do not reuse the existing Uswah content tables.
