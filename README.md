# 🥭 Mango Calculator

**The only financial tool that matters.**

> *How many mangoes is that, really?*

Convert any amount in any currency into its true value — kilograms of fresh Indian mangoes, priced live from real markets.

---

## What it does

You type £100. It tells you: **32.5 kg of mangoes** (~130 individual mangoes).

- Fetches the **live mango price** from Indian wholesale markets via [Agmarknet](https://data.gov.in) — averaged across all reported mandis
- Converts your currency to INR using **real-time exchange rates**
- Tells you exactly how many 250g mangoes you could hold in your arms

It also answers the important questions: how many mangoes is a Ferrari worth? A Big Mac? An espresso in Rome?

---

## Try it

**[→ Open the calculator](https://Carlo-Carpio.github.io/mango-calculator/)**

No install. No signup. One file.

---

## Why

Every price is abstract until you measure it in something real.

The mango is the world's most consumed fruit. It is grown by hand, sold in open markets, and priced daily by supply and demand. It is a better unit of value than most currencies.

---

## Stack

Pure HTML + CSS + JS. Zero dependencies. One file: `index.html`.

| Data source | What it provides |
|---|---|
| [data.gov.in / Agmarknet](https://data.gov.in/resource/current-daily-price-various-commodities-various-markets-mandi) | Live mango price (₹/kg), averaged across Indian mandis |
| [ExchangeRate-API](https://open.er-api.com) | Live currency → INR conversion |

---

## Run locally

```sh
git clone https://github.com/Carlo-Carpio/mango-calculator.git
cd mango-calculator
open index.html
```

That's it.

---

*Made with unreasonable enthusiasm for mangoes.*
