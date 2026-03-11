<div align="center">

# 💰 Expense Tracker

**A modern, elegant personal finance tracker — live on GitHub Pages with zero setup.**

[![Live Demo](https://img.shields.io/badge/🌐_Live_Demo-Visit_App-c9a84c?style=for-the-badge)](https://crafted-by-tarun.github.io/Expense-Tracker/)
[![GitHub Pages](https://img.shields.io/badge/Hosted_on-GitHub_Pages-222?style=for-the-badge&logo=github)](https://pages.github.com/)
[![React](https://img.shields.io/badge/React-18-61DAFB?style=for-the-badge&logo=react&logoColor=black)](https://react.dev/)
[![No Build](https://img.shields.io/badge/No_Build_Step-✓-4caf84?style=for-the-badge)]()

---

![Expense Tracker Screenshot](https://i.imgur.com/placeholder.png)

*Track your income and expenses beautifully — with real-time charts, categories, and local persistence.*

</div>

---

## ✨ Features

| Feature | Description |
|---|---|
| 💸 **Add Transactions** | Log income and expenses with descriptions and amounts |
| 🏷️ **12 Categories** | Food, Transport, Shopping, Health, Salary, Freelance, and more |
| 📊 **Live Balance** | Real-time total balance, income, and expense summary |
| ✏️ **Edit & Delete** | Modify or remove any transaction instantly |
| 🔍 **Search** | Filter transactions by description in real time |
| 🧩 **Filter by Type/Category** | Narrow down by income/expense or specific category |
| 🥧 **Pie Chart** | Visual spending breakdown by category |
| 📈 **Bar Chart** | Monthly income vs expense comparison (last 6 months) |
| 💾 **Auto-Save** | Data persists in browser LocalStorage across sessions |
| 📱 **Responsive** | Works beautifully on mobile, tablet, and desktop |

---

## 🚀 Live Demo

👉 **[crafted-by-tarun.github.io/Expense-Tracker](https://crafted-by-tarun.github.io/Expense-Tracker/)**

No login required. Your data is stored locally in your browser.

---

## 🖼️ Screenshots

<table>
  <tr>
    <td align="center"><b>Dashboard</b></td>
    <td align="center"><b>Add Transaction</b></td>
  </tr>
  <tr>
    <td><img src="https://i.imgur.com/placeholder1.png" width="400"/></td>
    <td><img src="https://i.imgur.com/placeholder2.png" width="400"/></td>
  </tr>
  <tr>
    <td align="center"><b>Pie Chart</b></td>
    <td align="center"><b>Bar Chart</b></td>
  </tr>
  <tr>
    <td><img src="https://i.imgur.com/placeholder3.png" width="400"/></td>
    <td><img src="https://i.imgur.com/placeholder4.png" width="400"/></td>
  </tr>
</table>

> 💡 **Tip:** Replace the placeholder image URLs above with real screenshots from your live app!

---

## 🗂️ Project Structure

```
Expense-Tracker/
├── index.html      ← The entire app (HTML + CSS + JS + React in one file)
└── README.md       ← This file
```

That's it — **just one HTML file**. No `node_modules`, no build process, no configuration.

---

## 🛠️ Tech Stack

| Technology | Purpose | How it's loaded |
|---|---|---|
| **React 18** | UI components & state management | CDN |
| **HTML5 Canvas** | Charts (Pie & Bar) — no library needed | Built-in |
| **CSS Variables** | Design tokens & theming | Inline |
| **LocalStorage API** | Data persistence | Built-in |
| **Google Fonts** | Playfair Display + DM Sans typography | CDN |

> **Why no build step?** Everything runs directly in the browser using React's UMD build from a CDN. This makes it trivially easy to host on GitHub Pages.

---

## 🏗️ How It Works

### State Management
All transaction data lives in a single custom `useTransactions()` hook that:
- Loads saved data from `localStorage` on first render
- Automatically syncs back to `localStorage` on every change
- Exposes clean `add`, `update`, `remove`, `startEdit`, `cancelEdit` functions

### Components
| Component | Role |
|---|---|
| `Header` | Sticky navbar with logo and live date |
| `Balance` | Hero card showing total balance, income, expenses |
| `AddTransaction` | Form for adding/editing transactions with validation |
| `TxList` | Searchable, filterable transaction history |
| `TxItem` | Individual transaction row with edit/delete |
| `Chart` | Analytics panel — toggles between Pie and Bar views |
| `PieCanvas` | Donut chart drawn with HTML5 Canvas |
| `BarCanvas` | Grouped bar chart drawn with HTML5 Canvas |

### Data Flow
```
useTransactions() hook
       │
       ├── transactions[]  ──→  Balance, TxList, Chart
       ├── editing tx      ──→  AddTransaction (pre-fills form)
       └── CRUD functions  ←──  All components via props
```

---

## 📋 Categories

**Expense categories**
> 🍜 Food & Dining · 🚗 Transport · 🛍️ Shopping · 🏠 Housing · 💊 Health · 📚 Education · ✈️ Travel · 🎮 Entertainment · 📦 Other

**Income categories**
> 💼 Salary · 💻 Freelance · 📈 Investment · 📦 Other

---

## 📦 How to Use Locally

No terminal needed — just open the file:

1. Download `index.html`
2. Double-click to open in any browser
3. Start tracking! ✅

---

## ☁️ How to Deploy Your Own Copy

1. **Fork** this repository (click Fork at the top right)
2. Go to **Settings → Pages**
3. Set Source to **Deploy from a branch → main → / (root)**
4. Click **Save**
5. Your app is live at `https://YOUR-USERNAME.github.io/Expense-Tracker/`

---

## 🤝 Contributing

Contributions are welcome! Feel free to:
- 🐛 Report bugs by opening an [Issue](../../issues)
- 💡 Suggest features
- 🔧 Submit a Pull Request

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

<div align="center">

Made with ❤️ by [crafted-by-tarun](https://github.com/crafted-by-tarun)

⭐ **Star this repo if you found it useful!**

</div>
