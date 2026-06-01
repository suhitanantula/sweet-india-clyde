# 🍬 Sweet India Clyde — WhatsApp Smart Campaigns

> Turn WhatsApp into the most powerful marketing channel for Sweet India Clyde. Festival specials, weather-triggered promotions, and weekly deals — all from one dashboard.

**Live Demo:** [sweet-india-clyde.vercel.app](https://sweet-india-clyde.vercel.app) *(deploy pending)*

---

## What Is This?

A phased system to help **Sweet India Clyde** (Indian restaurant/sweet shop in Clyde, Victoria) send smart, context-driven WhatsApp broadcasts to their customers.

**Right now:** Phase 0 — an interactive demo showing 5 campaign scenarios that a restaurant owner can see, click through, and immediately understand.

---

## 🎯 The Vision

### Phase 0 — The Demo ✅ *(Current)*
Something tangible to put in front of the client before any money changes hands.

- 5 campaign scenarios with live WhatsApp simulation
- Campaign selector panel to switch between scenarios
- Dynamic message preview with products, pricing, and customer conversation
- Weather context badge (Rainy Day Chai shows live Clyde weather)

**Campaigns included:**
| Campaign | Emoji | Segment | Products |
|----------|-------|---------|----------|
| Diwali 2026 | 🪔 | All Customers (2,847) | Sweet boxes, hampers, corporate gifts |
| Rainy Day Chai | 🌧️ | Weather-triggered locals (1,264) | Chai combos, samosa platters, vada pav |
| Eid Mubarak | 🌙 | Festival family buyers (1,936) | Biryani packs, sheer khurma, haleem |
| Holi Colour Fest | 🎨 | Festival sweet lovers (2,218) | Thandai, gujiya, sweet assorted |
| Weekend Special | 🍛 | Weekend dinner customers (3,152) | Butter chicken, paneer tikka, family feast |

**Cost:** $0–300 | **Time:** Done | **Deliverable:** Shareable link

---

### Phase 1 — Foundation *(Next)*
Get the first real broadcast sent to real customers.

**WhatsApp Business API setup:**
- Register business number with Meta Business Manager
- Onboard API platform (WATI, Interakt, or AiSensy)
- Submit 3 message templates for Meta approval (Diwali promo, weather special, weekly)
- Connect business phone number

**Contact list:**
- Audit existing contacts (saved phones, spreadsheets, loyalty app)
- Clean and import: Name, Phone, Tags
- Set up opt-in flow (QR code on counter → WhatsApp opt-in message)

**First broadcast:**
- Run Diwali campaign using scripted templates from demo
- Monitor delivery, read, and click stats
- Document what worked

| Item | Cost |
|------|------|
| WATI or Interakt platform | A$50–80/month |
| Meta per-conversation fee (~2,800 contacts) | A$140–200 per broadcast |
| Setup and onboarding | A$800–1,500 one-off |
| **Phase 1 total (first month)** | **~A$1,000–1,800** |

**Time:** 3–4 weeks (Meta verification is the bottleneck)

---

### Phase 2 — Campaign Builder
Owner creates and sends context-driven campaigns in under 5 minutes.

**What gets built:**
- **Campaign Builder UI** — Pick event/festival + weather + segment, see live preview
- **Weather integration** — OpenWeatherMap for Clyde (3978), auto-suggest "Chai & Samosa" when cold/rain
- **Festival calendar** — JSON calendar for Indian/multicultural dates 2026–2027, 14-day and 7-day alerts
- **Template library** — 6–8 Meta-approved templates with auto-filled variables
- **Backend** — Node.js or Python server on Railway/Render

| Item | Cost |
|------|------|
| Full-stack build | A$4,000–6,500 |
| Hosting (Railway/Render) | A$15–20/month |
| Platform (WATI/Interakt) | A$50–80/month |
| **Monthly running** | **~A$65–100 + broadcast fees** |

**Time:** 5–7 weeks

---

### Phase 3 — Automation & Intelligence
Set-and-forget. System watches weather and calendar, prompts owner or sends with approval.

**What gets built:**
- **Automated weather triggers** — 7am check, push notification if rain/cold, one-tap approve
- **Segment intelligence** — Connect POS/order history, auto-tag regulars/corporate/lapsed
- **A/B testing** — Two message variants to 10%, best performer auto-sends to rest
- **Analytics dashboard** — Best campaigns, best times, revenue per broadcast
- **Scheduling** — Queue campaigns ahead, optimised send times

| Item | Cost |
|------|------|
| Development | A$10,500–13,500 |
| POS integration (if needed) | A$500–1,500 extra |
| Enhanced hosting | A$30–50/month |
| **Monthly running** | **~A$110–200 + broadcast fees** |

**Time:** 8–12 weeks

---

## 💰 Total Investment Summary

| Phase | Client Gets | Build Cost | Monthly |
|-------|-------------|------------|---------|
| 0 — Demo | Something to say yes to | $0–300 | $0 |
| 1 — Foundation | Real broadcasts, contacts, first campaign | $800–1,500 | $190–280 |
| 2 — Campaign Builder | Owner-driven smart campaigns | $4,000–6,500 | $65–100 |
| 3 — Automation | Set-and-forget intelligence | $10,500–13,500 | $110–200 |
| **Full build** | | **$15,000–22,000** | **~$300–480** |

---

## 📊 The Business Case

A single Diwali broadcast to 2,800 customers, if **5% convert** at average order **A$50**:

> **A$7,000 revenue from one send.** Broadcast cost: ~A$200. **35x return.**

Run 2–3 campaigns/month (festivals, weather, weekly deals) and even at half performance, the system pays for itself within 2–3 months of Phase 2 going live.

---

## 🛠 Tech Stack

| Layer | Choice | Why |
|-------|--------|-----|
| Demo | HTML/CSS/JS (single file) | Zero dependencies, shareable link |
| WhatsApp API | WATI / Interakt / AiSensy | Australian support, template management |
| Backend | Node.js or Python (FastAPI) | Lightweight, Railway/Render hosting |
| Weather | OpenWeatherMap API | Free tier (1,000 calls/day) |
| Database | Supabase (Phase 3) | Contacts, segments, analytics |
| Hosting | Railway or Render | A$15–20/month, auto-deploy |

---

## 📁 Project Structure (Current — Phase 0)

```
sweet-india-clyde/
├── index.html          # The complete demo (1,227 lines, zero dependencies)
├── README.md           # This file — full project vision
├── ROADMAP.md          # Detailed phase breakdown
└── docs/
    ├── api-platforms-comparison.md  # WATI vs Interakt vs AiSensy
    ├── meta-template-guide.md       # How to get templates approved
    └── campaign-scripts/            # All 5 campaign message scripts
        ├── diwali.md
        ├── rainy-day-chai.md
        ├── eid-mubarak.md
        ├── holi-colour-fest.md
        └── weekend-special.md
```

---

## 🚀 Quick Start

```bash
# Just open the demo
open index.html

# Or serve it locally
python3 -m http.server 8000
# → http://localhost:8000
```

---

## Client Recommendation

> Start with Phase 0 — show them the demo. Then propose Phase 1 only, framed as a pilot: *"Let's get one real campaign out the door, measure what happens, and then decide what to build next."*
>
> Keep the commitment small and the first win fast. **Diwali 2026 is the perfect anchor.**

---

## Contact

**Developer:** Amit (via Suhit Anantula / The Helix Lab)
**Client:** Sweet India Clyde, Clyde VIC 3978

---

*Built with ❤️ for Sweet India Clyde*
