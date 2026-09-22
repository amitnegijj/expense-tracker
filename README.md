# Finance Tracker

A React-based personal finance tracker app to manage and visualize your income and expenses.

## Features

- 📊 Real-time summary of **Income**, **Expenses**, and **Balance**
- ➕ Add new transactions with description, amount, type, and category
- 🔍 Filter transactions by type and category
- 🧩 Clean component-based architecture

## Tech Stack

- [React 19](https://react.dev/)
- [Vite](https://vitejs.dev/)
- Vanilla CSS

## Project Structure

```
src/
├── App.jsx              # Root component — holds transactions state
├── Summary.jsx          # Calculates & displays income/expense/balance
├── TransactionForm.jsx  # Form to add new transactions
├── TransactionList.jsx  # Filterable transaction table
├── App.css              # Styles
└── main.jsx             # Entry point
```

## Getting Started

```bash
npm install
npm run dev
```

Then open your browser at `http://localhost:5173`.

## Bug Fixes Applied

- Fixed incorrect income/expense totals caused by string amounts being concatenated instead of summed
- Converted all hardcoded transaction `amount` values from strings to numbers
- more to come 

## Refactoring Done

- Extracted `Summary`, `TransactionForm`, and `TransactionList` into separate components
- Moved financial calculations into `Summary` component
- Moved form state into `TransactionForm` component
- Moved filter state into `TransactionList` component
- `App.jsx` now only manages shared `transactions` state
