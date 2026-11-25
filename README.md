# Expense Tracker — React + Vite

A polished personal finance tracker built with React, Vite, Recharts and Lucide icons.

## Run locally
1. Install Node.js (LTS).
2. Extract this ZIP and open the `Expense Tracker-React` folder in VS Code.
3. Open a terminal in that folder and run:
   ```bash
   npm install
   npm run dev
   ```
4. Open the local URL printed by Vite (usually http://localhost:5173).

## Production build
```bash
npm run build
npm run preview
```
Deploy the project folder to Vercel (Framework Preset: Vite; Build Command: `npm run build`; Output Directory: `dist`).

## Features
- Marketing landing page before login; separate sign-in and registration screens.
- Dashboard summary cards, recent transactions, category pie chart and financial-year income/expense bar chart.
- Select FY 2023–24, 2024–25 or 2025–26 to see that year's income, expenses and net savings.
- Transactions, monthly budget, savings goals, recurring expenses, accounts and reports.
- Responsive layout for desktop and mobile.
- Uses browser Local Storage for persistence.

## Existing project data
The app reads the existing Local Storage keys used by the previous HTML/JS project:
`expenses`, `incomes`, `goals`, `accounts`, `recurringExpenses`, `monthlyBudget`, and `user`.
If the same browser profile is used, existing records can be reused automatically. Records are not moved between different browsers/devices.

## Important
This is a front-end demo. Authentication and data are stored in browser Local Storage, not a secure backend. Do not use real passwords or sensitive financial information. Financial-year charts are calculated from transaction dates (April 1 to March 31); years without records correctly show zero rather than invented figures.
