# Realtor Lead Master

Searchable, deduped warehouse of **2,571,615 unique leads** consolidated from 9 GoHighLevel subaccounts (1PM Collective).

- **Live app:** https://realtor-leads.1pm.ai (login required)
- **Source:** 4,205,294 raw contacts across Instagram, ChatGPT Bookings, Costar, 1PropertyMarket, Zillow, Realtor.com, eXp, Loopnet, 1PM AI — deduped by phone number.
- **Backend:** Supabase (`lm_contacts`, `lm_smart_lists`). Reads require an authenticated, allowlisted login (Row Level Security). The anon key in `index.html` cannot read leads on its own.
- **Features:** full-text search, filters (subaccount, tag, has phone/email, cross-account), sort, persistent saved smart lists, contact profile with per-source GoHighLevel deep links and prev/next navigation, CSV export.

Single static file (`index.html`) hosted via GitHub Pages. To add team logins, insert their email into `public.lm_allowed_emails` and create their Supabase Auth user.
