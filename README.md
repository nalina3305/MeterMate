# Dorm Meter Tracker

A single-page web app that helps students living in dorms and rented rooms log their electricity and water meter readings and see right away when they are using more than usual, before the monthly bill arrives.

## The problem

Many dorms and rentals charge for electricity and water by meter, but residents only learn the total when the bill arrives. By then it is too late to react: an air conditioner left on during exam week, a leaking tap, or a running toilet has already cost money. Without a history to compare against, there is also no way to tell whether a bill is normal.

## Who it is for

Students and tenants who pay for electricity and water by meter and want to keep their monthly costs under control. Defaults are Thai baht (8 per kWh of electricity, 18 per m³ of water), and you can change the currency and prices to match your own bill.

## What it does

- Log electricity (kWh) and water (m³) meter readings, for example once a week
- Calculates daily usage and cost from your own prices
- Warns you when the latest period is above your normal usage by more than a threshold you choose (default 30%)
- Shows usage per day in a chart and estimates the full monthly bill
- Validates entries (a reading can't be lower than the previous one)
- Stores everything in your browser (localStorage). Nothing is uploaded.

## How to run

No installation needed. Pick one:

1. Double-click `index.html` to open it in a browser.
2. Or run a local server in this folder: `python -m http.server 8000`, then open http://localhost:8000

An internet connection is needed to load Chart.js. Offline, the numbers and warnings still work but the charts won't show.

## Try it quickly

Click **Load sample data** to see five weeks of readings where electricity use jumps in the latest week because the air conditioner was left on. Then set your own currency and prices in **Settings** and start logging real readings.

## Built with

HTML, CSS, JavaScript, and [Chart.js](https://www.chartjs.org/)

## Notes

Solo project for the "Solve a Real Problem" challenge (solo alternative to the Creative Coding Hackathon).
