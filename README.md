# Expense Tracker Web App

A simple and responsive web application to track personal income and expenses. Built with pure HTML, CSS, and JavaScript—no backend needed.

## Features
- Add income or expense entries with description and amount.
- View a detailed transaction history list.
- Displays current balance, total income, and total expenses.
- Delete transactions effortlessly.
- Persist data in browser using **LocalStorage**, so your entries remain after refresh or browser restart.
- Clean and responsive user interface, making it mobile-friendly.

## How It Works

1. **UI Structure (`index.html`)**
   - Input form: description + amount (positive for income, negative for expense).
   - Displays current balance, income, expense breakdown.
   - Transaction list showing each entry with a delete button.

2. **Styling (`style.css`)**
   - Uses CSS flexbox/grid and media queries for responsive design.
   - Simple, clean layout for readability.

3. **Logic (`script.js`)**
   - Initializes `transactions` array from LocalStorage or empty if none.
   - `updateUI()`:
     - Clears and rebuilds transaction list.
     - Computes balance, income, and expense totals.
     - Saves the updated array back to LocalStorage.
   - Form submission handler:
     - Reads user input, creates a transaction `{description, amount}`, appends to array, resets form, calls `updateUI()`.
   - Delete button handler:
     - Removes the selected entry based on index, updates the UI.


Let me know what you'd like next!
::contentReference[oaicite:0]{index=0}
