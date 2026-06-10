# Mango Calculator

A single-page web app that converts any currency into kilograms of Indian mangoes.
No build step, no dependencies, no backend — everything lives in `index.html`.

## Structure

```
mango-calculator/
├── index.html   # entire app — HTML + CSS + JS in one file
└── README.md
```

## How it works

1. On page load, fetches live mango prices from **data.gov.in** (Agmarknet daily commodity prices, ₹/quintal → divided by 100 to get ₹/kg). Falls back to ₹100/kg if the API is unavailable.
2. On convert, fetches live exchange rates from **open.er-api.com** to convert the selected currency to INR.
3. Divides the INR amount by the mango price to get kg, then estimates individual mangoes at ~250g each.

## APIs (no API key required)

- Mango prices: `https://api.data.gov.in/resource/9ef84268-d588-465a-a308-a864a43d0070?api-key=579b464db66ec23bdd000001cdd3946e44ce4aab108d4753e6d8f3b6&format=json&filters[commodity]=Mango&limit=100`
- Exchange rates: `https://open.er-api.com/v6/latest/{currency}`

## Supported currencies

GBP, USD, EUR, CHF, AUD, CAD, JPY, INR

## Hosting

Deployed as a static site on GitHub Pages. No server needed.
To run locally: `python3 -m http.server 8080` (do not open via `file://` — CORS errors).
