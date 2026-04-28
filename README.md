# 💰 Expense Tracker

A clean, modern, and fully responsive **Expense Tracker** web application that helps you manage your personal finances with ease. Track your income and expenses, view your balance in real-time, and keep a complete history of all your transactions — all stored locally in your browser.

<p align="center">
  <a href="https://expense-tracker2002.netlify.app/" target="_blank">
    <img src="https://img.shields.io/badge/Live%20Demo-View%20Site-brightgreen?style=for-the-badge&logo=netlify" alt="Live Demo" />
  </a>
  <a href="https://github.com/razazaheer12/EXPENSE_TRACKER" target="_blank">
    <img src="https://img.shields.io/badge/GitHub-Repository-blue?style=for-the-badge&logo=github" alt="GitHub Repo" />
  </a>
</p>

---

## 📸 Preview

![Expense Tracker Preview](https://via.placeholder.com/800x450/2e8b57/ffffff?text=Expense+Tracker+Preview)

> **Live URL:** [https://expense-tracker2002.netlify.app/](https://expense-tracker2002.netlify.app/)

---

## ✨ Features

| Feature | Description |
|---------|-------------|
| ➕ **Add Transactions** | Quickly add income or expenses with a description and amount. |
| 📊 **Real-Time Balance** | Instantly see your current balance calculated from all transactions. |
| 💵 **Income Tracking** | View total income separately with green highlighting. |
| 💸 **Expense Tracking** | View total expenses separately with red highlighting. |
| 📝 **Transaction History** | See a complete list of all your past transactions with timestamps. |
| 🗑️ **Delete Transactions** | Remove any transaction with a single click. |
| 💾 **Local Storage** | All data is saved in your browser — no account needed, no data lost on refresh. |
| 📱 **Fully Responsive** | Works seamlessly on desktop, tablet, and mobile devices. |
| 🎨 **Modern UI** | Clean gradient design with smooth animations and hover effects. |
| 💲 **Currency Formatting** | Automatic USD currency formatting for all amounts. |

---

## 🛠️ Tech Stack

<p align="left">
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5" />
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" alt="CSS3" />
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript" />
  <img src="https://img.shields.io/badge/Netlify-00C7B7?style=for-the-badge&logo=netlify&logoColor=white" alt="Netlify" />
</p>

- **HTML5** — Semantic structure and accessibility
- **CSS3** — Modern styling with Flexbox, Grid, gradients, animations, and responsive design
- **Vanilla JavaScript** — No frameworks, pure DOM manipulation and localStorage API
- **Netlify** — Fast and reliable static site hosting

---

## 🚀 Getting Started

### Prerequisites

You only need a modern web browser to run this project locally. No build tools or dependencies required!

### Installation

1. **Clone the repository**

   ```bash
   git clone https://github.com/razazaheer12/EXPENSE_TRACKER.git
   ```

2. **Navigate to the project folder**

   ```bash
   cd EXPENSE_TRACKER
   ```

3. **Open in browser**

   Simply open the `index.html` file in your favorite browser:

   ```bash
   # On Windows
   start index.html

   # On macOS
   open index.html

   # On Linux
   xdg-open index.html
   ```

   Or use a live server extension in VS Code for the best development experience.

---

## 📖 How to Use

1. **Add an Income** — Enter a description (e.g., "Freelance Payment") and a **positive** amount, then click **Add Transaction**.
2. **Add an Expense** — Enter a description (e.g., "Groceries") and a **negative** amount (e.g., `-50`), then click **Add Transaction**.
3. **View Summary** — Your total balance, income, and expenses will update automatically at the top.
4. **Manage History** — All transactions appear in the list. Hover over any transaction and click the **×** button to delete it.
5. **Persistent Data** — Your transactions are saved automatically. Close and reopen the browser — your data will still be there!

---

## 📁 Project Structure

```
EXPENSE_TRACKER/
│
├── index.html          # Main HTML structure
├── style.css           # All styles, animations, and responsive queries
├── index.js            # Application logic, localStorage, and DOM updates
└── README.md           # Project documentation
```

### File Overview

| File | Purpose |
|------|---------|
| `index.html` | Defines the app layout including balance dashboard, transaction list, and input form. |
| `style.css` | Provides a modern, gradient-based design with smooth animations, custom scrollbar, and full mobile responsiveness. |
| `index.js` | Handles all interactivity: adding/deleting transactions, calculating totals, formatting currency, and persisting data to `localStorage`. |

---

## 🎯 Key Functionalities

### Balance Calculation
```javascript
const balance = transactions.reduce((acc, transaction) => acc + transaction.amount, 0);
```

### Income & Expense Separation
```javascript
const income = transactions.filter(t => t.amount > 0).reduce((acc, t) => acc + t.amount, 0);
const expenses = transactions.filter(t => t.amount < 0).reduce((acc, t) => acc + t.amount, 0);
```

### Data Persistence
```javascript
// Save to localStorage
localStorage.setItem("transactions", JSON.stringify(transactions));

// Load from localStorage
let transactions = JSON.parse(localStorage.getItem("transactions")) || [];
```

---

## 📱 Responsive Design

The application is fully responsive and adapts beautifully to all screen sizes:

- **Desktop (1200px+)** — Two-column layout with transaction list on the left and form on the right.
- **Tablet (900px)** — Stacks into a single column for better readability.
- **Mobile (480px)** — Compact layout with full-width cards, larger touch targets, and optimized typography.

---

## 🎨 Design Highlights

- 🌿 **Green Gradient Theme** — Inspired by financial growth and prosperity.
- ✨ **Smooth Animations** — Slide-in effects for new transactions and hover transforms.
- 🖱️ **Interactive Elements** — Buttons and cards respond to hover and click with subtle animations.
- 🎚️ **Custom Scrollbar** — Styled scrollbar for the transaction list on WebKit browsers.
- 🏷️ **Color-Coded Transactions** — Green border for income, red border for expenses.

---

## 🔮 Future Enhancements

- [ ] Edit existing transactions
- [ ] Filter transactions by date or category
- [ ] Export data to CSV or PDF
- [ ] Dark mode toggle
- [ ] Multi-currency support
- [ ] Charts and visual analytics (pie chart, bar graph)
- [ ] Cloud sync with user authentication

---

## 🤝 Contributing

Contributions are welcome! If you have suggestions, bug fixes, or new features to add:

1. Fork the repository
2. Create a new branch (`git checkout -b feature/YourFeature`)
3. Commit your changes (`git commit -m 'Add some feature'`)
4. Push to the branch (`git push origin feature/YourFeature`)
5. Open a Pull Request

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

## 🙏 Acknowledgments

- Built with ❤️ by [Raza Zaheer](https://github.com/razazaheer12)
- Hosted on [Netlify](https://www.netlify.com/)
- Font: [Poppins](https://fonts.google.com/specimen/Poppins) by Google Fonts

---

<p align="center">
  <b>⭐ Star this repo if you found it helpful!</b>
</p>

<p align="center">
  <a href="https://expense-tracker2002.netlify.app/">🌐 Live Demo</a> •
  <a href="https://github.com/razazaheer12/EXPENSE_TRACKER">💻 GitHub Repo</a>
</p>

