# 🗺️ Roadmap — Sweet India Clyde WhatsApp Smart Campaigns

---

## Phase 0: The Demo — ✅ COMPLETE

**Goal:** Tangible demo to show the client before any money changes hands.

### What was built
- [x] WhatsApp phone mockup with 5-step animated demo
- [x] Campaign Builder selector panel (5 campaigns)
- [x] Dynamic content switching (messages, products, pricing, order flow)
- [x] Live delivery stats with animated counters
- [x] Customer journey log
- [x] Weather context badge for Rainy Day campaign
- [x] Responsive design (mobile + desktop)
- [x] Single `index.html`, zero dependencies

### 5 Campaigns
1. **Diwali 2026** — 🪔 — All Customers (2,847) — Sweet boxes & hampers
2. **Rainy Day Chai Special** — 🌧️ — Weather-triggered (1,264) — Chai, samosa, vada pav
3. **Eid Mubarak** — 🌙 — Festival families (1,936) — Biryani, sheer khurma, haleem
4. **Holi Colour Fest** — 🎨 — Festival sweet lovers (2,218) — Thandai, gujiya, sweets
5. **Weekend Special** — 🍛 — Weekend dinners (3,152) — Butter chicken, family feast

### Deliverable
- Shareable link (GitHub Pages or Vercel)
- Client sees exactly what they'd get

---

## Phase 1: Foundation — 📋 READY TO START

**Goal:** First real broadcast sent to real customers.

### Prerequisites (client must provide)
- [ ] Business phone number (dedicated or shared)
- [ ] Business registration details (ABN)
- [ ] Facebook Business Manager account (or willingness to create one)
- [ ] Existing contact list (phones, names, any tags)
- [ ] Business logo and brand assets

### Step 1.1: Meta Business Setup (Week 1–2)
- [ ] Register business with Meta Business Manager
- [ ] Verify business (document upload, phone verification)
- [ ] Create WhatsApp Business Account
- [ ] Add business phone number

### Step 1.2: API Platform Onboarding (Week 1–2, parallel)
- [ ] Evaluate platforms: WATI vs Interakt vs AiSensy
- [ ] Sign up for chosen platform
- [ ] Connect WhatsApp Business Account
- [ ] Configure business profile (name, logo, address, hours)

### Step 1.3: Template Approval (Week 2–3)
- [ ] Draft 3 message templates:
  - [ ] Diwali promotional template
  - [ ] Weather special template
  - [ ] General weekly deal template
- [ ] Submit to Meta for approval
- [ ] Iterate if rejected (common reasons: too promotional, missing opt-out)

### Step 1.4: Contact List (Week 2–3, parallel)
- [ ] Audit existing contacts (phone contacts, spreadsheet, loyalty app, nothing)
- [ ] Clean data: standardise phone format (+61), remove duplicates
- [ ] Import into platform with tags (regular, corporate, lapsed, new)
- [ ] Design and print QR code for counter opt-in
- [ ] Set up automated welcome message for new opt-ins

### Step 1.5: First Broadcast (Week 3–4)
- [ ] Select campaign (Diwali recommended — biggest impact)
- [ ] Final check: template approved, contacts imported, timing set
- [ ] Send broadcast during optimal window (10–11am for food)
- [ ] Monitor: delivery rate, read rate, click rate, replies
- [ ] Document everything: what worked, what didn't, customer responses

### Phase 1 Success Metrics
- [ ] 90%+ delivery rate
- [ ] 60%+ read rate
- [ ] 5%+ click/engagement rate
- [ ] At least 10 orders attributed to broadcast
- [ ] Client comfortable checking dashboard

---

## Phase 2: Campaign Builder — 🔮 FUTURE

**Goal:** Owner creates and sends campaigns themselves in under 5 minutes.

### Frontend — Campaign Builder UI
- [ ] Web-based dashboard (React or vanilla JS)
- [ ] Campaign type selector (festival, weather, weekly, custom)
- [ ] Product/offer picker with pricing
- [ ] Live WhatsApp message preview
- [ ] Segment selector (all, regulars, lapsed, new, weather-triggered)
- [ ] Send now / Schedule / Save as draft
- [ ] Template variable auto-fill ({{name}}, {{product}}, {{price}})

### Weather Integration
- [ ] Connect OpenWeatherMap API for Clyde VIC 3978
- [ ] Daily weather fetch (temperature, conditions, rainfall)
- [ ] Auto-suggest triggers:
  - Below 15°C → "Chai & Samosa" campaign suggestion
  - Rain detected → "Rainy Day Comfort" campaign suggestion
  - Above 35°C → "Cool Drinks & Light Meals" suggestion
- [ ] Weather context displayed on dashboard
- [ ] Historical weather data for send time optimisation

### Festival Calendar
- [ ] JSON/DB calendar with 2026–2027 multicultural dates:
  - Diwali, Holi, Eid al-Fitr, Eid al-Adha, Navratri, Ganesh Chaturthi
  - Christmas, Easter, Australia Day, New Year
  - Regional/community events
- [ ] 14-day alert: "Diwali is in 14 days — schedule your campaign?"
- [ ] 7-day alert: "Diwali is in 7 days — ready to send?"
- [ ] 1-day reminder
- [ ] Owner can add custom dates (store anniversary, community events)

### Template Library
- [ ] 6–8 pre-written, Meta-approved templates
- [ ] Variable auto-fill from selector choices
- [ ] Preview with sample customer data
- [ ] A/B variant field for testing

### Backend
- [ ] API server (Node.js or Python FastAPI)
- [ ] Campaign orchestrator (weather check → calendar check → template fill → send)
- [ ] Contact segment engine
- [ ] Send queue and scheduler
- [ ] Basic auth for dashboard access
- [ ] Deploy to Railway or Render

### Phase 2 Deliverables
- [ ] Working Campaign Builder dashboard
- [ ] Weather-triggered suggestions live
- [ ] Festival calendar with alerts
- [ ] Owner can create and send a campaign in under 5 minutes
- [ ] Documentation and walkthrough video

---

## Phase 3: Automation & Intelligence — 🔮 FUTURE

**Goal:** Set-and-forget. Owner spends 2 minutes/day, not 20.

### Automated Weather Triggers
- [ ] Scheduled 7am daily weather check
- [ ] If trigger condition met → push notification to owner's phone
- [ ] Owner gets WhatsApp message: "🌧️ Rain in Clyde today. Send Chai campaign?"
- [ ] One-tap approve or dismiss
- [ ] Auto-send approved campaign to weather-triggered segment

### Segment Intelligence
- [ ] Connect POS system (Square, Shopify, or manual spreadsheet)
- [ ] Auto-tagging rules:
  - Regular: 3+ orders in 90 days
  - Corporate: single order over A$200
  - Lapsed: no order in 60+ days
  - New: opted in but no order yet
  - High-value: average order > A$100
- [ ] Different message variants per segment
- [ ] Segment-specific sending times

### A/B Testing
- [ ] Create two message variants
- [ ] Send to 10% of list (5% each variant)
- [ ] Track opens, clicks, replies for 2 hours
- [ ] Auto-send winner to remaining 90%
- [ ] Results stored for learning

### Analytics Dashboard
- [ ] Campaign performance table (sent, delivered, read, clicked, converted)
- [ ] Revenue attribution (broadcast click → order data)
- [ ] Best sending times chart (by hour, by day)
- [ ] Segment performance comparison
- [ ] Month-over-month trends
- [ ] Simple export (CSV/PDF)

### Scheduling & Optimisation
- [ ] Queue campaigns up to 2 weeks ahead
- [ ] Smart send time: system picks optimal hour based on past data
- [ ] Avoid overlap: minimum 48 hours between broadcasts to same segment
- [ ] Holiday/blackout periods

### Phase 3 Deliverables
- [ ] Automated weather triggers live
- [ ] Segment engine connected to POS
- [ ] A/B testing framework
- [ ] Analytics dashboard
- [ ] Smart scheduling
- [ ] Owner training session

---

## Key Decisions to Make

| Decision | Options | Recommendation | When |
|----------|---------|----------------|------|
| API Platform | WATI / Interakt / AiSensy | WATI (best template tools) | Phase 1 |
| Phone Number | Dedicated / Shared | Dedicated (looks more professional) | Phase 1 |
| First Campaign | Diwali / Weather / Weekly | Diwali (biggest ROI anchor) | Phase 1 |
| Backend Stack | Node.js / Python | Python FastAPI (lighter for this scope) | Phase 2 |
| Frontend | React / Vanilla / No-code | Start vanilla, upgrade if needed | Phase 2 |
| POS Integration | Square / Shopify / Manual | Depends on client's current system | Phase 3 |
| Hosting | Railway / Render / Vercel | Railway (simple, cheap) | Phase 2 |

---

## Risk Register

| Risk | Impact | Likelihood | Mitigation |
|------|--------|------------|------------|
| Meta rejects templates | High | Medium | Submit 5+ variants, follow guidelines closely |
| Contact list is messy | Medium | High | Budget extra cleanup time, use phone validation |
| Owner doesn't use it | High | Medium | Phase 2 makes it dead simple, Phase 3 is autopilot |
| Low broadcast engagement | Medium | Low | A/B testing, segment targeting, timing optimisation |
| Client's POS doesn't integrate | Low | Low | Fallback to manual spreadsheet upload |
| WhatsApp policy changes | Medium | Low | Stay on Business API (not grey routes), monitor Meta updates |

---

*Last updated: June 2026*
