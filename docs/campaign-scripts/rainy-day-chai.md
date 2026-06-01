# 🌧️ Campaign Script: Rainy Day Chai Special

**Campaign:** Rainy Day Chai Special
**Segment:** Weather-triggered Clyde locals
**Contacts:** 1,264
**Template:** Rainy Chai v1
**Trigger:** Temperature below 15°C or rain detected in Clyde VIC 3978
**Optimal send time:** 11:00 AM (when people want a warm lunch)

---

## Broadcast Message

> Namaste! ☔
>
> Rain has arrived in Clyde, and Sweet India Clyde has the perfect cozy fix waiting for you.
>
> ☕ Chai + Samosa Combo — A$12
> ☕ Masala Chai — A$5
> 🥟 Samosa Platter (6pc) — A$15
> 🍔 Vada Pav (4pc) — A$14
>
> Warm up your afternoon with fresh chai, crispy snacks, and comfort food made for rainy weather. 🌧️

**CTA:** ☕ Order Chai Now

**Weather badge:** 🌧️ 14°C Clyde — Perfect chai weather!

---

## Customer Journey Simulation

### Customer replies:
> "Hi! Rainy day chai sounds perfect ☔"

### Business responds:
> "Hi Priya! ☕ Great timing.
>
> Today's rainy day menu is ready:
>
> 1️⃣ Chai + Samosa Combo — A$12
> 2️⃣ Masala Chai — A$5
> 3️⃣ Samosa Platter (6pc) — A$15
> 4️⃣ Vada Pav (4pc) — A$14
>
> Tell us what you would like and we will keep it hot for pickup. 😊"

### Customer orders:
> "Can I get 2 Chai + Samosa Combos and 1 Vada Pav pack please? ☕"

### Business confirms:
> "Perfect! Here's your order summary:
>
> ☕ Chai + Samosa Combo × 2 = A$24
> 🍔 Vada Pav (4pc) × 1 = A$14
> ━━━━━━━━━━━━━━
> **Total: A$38.00**
>
> 📅 Pickup: Today after 5:00 PM
> 📍 Sweet India Clyde
>
> Pay on pickup or pay now via the link below 👇"

### Order confirmed:
> "✅ **Order Confirmed!**
>
> Order #SI-RN-2184
> We will keep the chai hot and snacks crispy.
>
> Thank you Priya! Stay warm. ☔"

---

## Weather Trigger Logic

```
IF temp_clyde < 15 OR rain_detected = true:
  → Suggest "Rainy Day Chai" campaign
  → Target segment: weather-triggered Clyde locals
  → Auto-fill weather badge with live temperature
```

## Key Metrics
- **Target conversion:** 3–5% (weather-triggered has lower urgency but higher relevance)
- **Average order value:** A$20–40
- **Expected revenue:** A$750–1,250 per send
