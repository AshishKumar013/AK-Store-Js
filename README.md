# 🛒 AK Store — JavaScript E-Commerce Application

<div align="center">

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white)
![Netlify](https://img.shields.io/badge/Netlify-00C7B7?style=for-the-badge&logo=netlify&logoColor=white)

**A fully responsive, multi-page e-commerce platform built from scratch with Modern JavaScript.**

[🌐 Live Demo](https://ecommjs.netlify.app/) 

</div>

---

## 📌 Overview

AK Store is a feature-rich, client-side e-commerce application built entirely with Vanilla JavaScript (ES6+), HTML5, and CSS3 — no frameworks, no libraries. It demonstrates core front-end engineering skills including dynamic DOM manipulation, persistent state management via the LocalStorage API, complex cart logic, and a clean, responsive UI across all devices.

---

## ✨ Features

- **Dynamic Product Rendering** — Products are fetched and rendered dynamically from a local API, with real-time UI updates.
- **Product Filtering** — Users can filter and browse products seamlessly without page reloads.
- **Shopping Cart System** — Full cart functionality including add, remove, quantity increment/decrement, and real-time price updates.
- **Persistent Cart State** — Cart data is stored in `LocalStorage`, ensuring items persist across browser sessions and page refreshes.
- **Accurate Price Calculations** — Sub-totals, shipping fees, and tax amounts are computed accurately and kept in sync with cart state at all times.
- **Toast Notifications** — Custom-built toast alerts provide instant, non-intrusive feedback on user actions (e.g., item added, item removed).
- **Interactive Animations** — Smooth UI transitions and animations enhance the overall user experience.
- **Fully Responsive Design** — Optimized layout for mobile, tablet, and desktop viewports.
- **Multi-Page Architecture** — Separate pages for Home, Products, Cart, About, and Contact.

---

## 🗂️ Project Structure

```
AK-Store-Js/
│
├── api/                          # Local product data / mock API
├── public/                       # Static assets (images, icons)
│
├── index.html                    # Home page
├── products.html                 # Products listing page
├── addToCart.html                # Shopping cart page
├── about.html                    # About page
├── contact.html                  # Contact page
│
├── main.js                       # App entry point
├── homeProductCards.js           # Renders product cards on home page
├── homeQuantityToggle.js         # Quantity toggle logic on home page
├── addToCart.js                  # Add-to-cart handler
├── getCartProducts.js            # Fetches cart items from LocalStorage
├── showAddToCartCards.js         # Renders cart item cards
├── fetchQuantityFromCartLS.js    # Syncs quantity state from LocalStorage
├── incrementDecrement.js         # Cart quantity increment/decrement logic
├── updateCartProductTotal.js     # Updates individual product totals in cart
├── updateCartValue.js            # Recalculates overall cart value (subtotal, tax, shipping)
├── removeProdFromCart.js         # Removes a product from the cart
├── showToast.js                  # Custom toast notification utility
├── footer.js                     # Dynamic footer rendering
│
├── style.css                     # Global styles
├── vite.config.js                # Vite build configuration
├── package.json
└── .gitignore
```

---

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| **HTML5** | Page structure and semantic markup |
| **CSS3** | Styling, animations, and responsive layouts |
| **JavaScript (ES6+)** | Application logic, DOM manipulation, state management |
| **LocalStorage API** | Client-side data persistence for cart state |
| **Vite** | Build tool with fast HMR for development |
| **Netlify** | Deployment and hosting |

---

## 🚀 Getting Started

### Prerequisites

- JavaScipt(ES6+)
- CSS
- Vite

### Installation & Local Development

1. **Clone the repository**
   ```bash
   git clone https://github.com/AshishKumar013/AK-Store-Js.git
   cd AK-Store-Js
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Start the development server**
   ```bash
   npm run dev
   ```

4. Open your browser and navigate to `http://localhost:5173`

### Production Build

```bash
npm run build
```

The optimized output will be generated in the `dist/` folder, ready for deployment.

---

## 📦 Deployment

This project is deployed on **Netlify** with continuous delivery. Every push to the `main` branch triggers an automatic build and deploy.

🔗 **Live URL:** [https://ecommjs.netlify.app/](https://ecommjs.netlify.app/)

---

## 💡 Key Implementation Highlights

**State Management without a Framework** — All cart state is managed manually using the `LocalStorage` API. A suite of dedicated JS modules (`getCartProducts.js`, `fetchQuantityFromCartLS.js`, `updateCartValue.js`) work together to keep the UI perfectly in sync with stored data.

**Modular JavaScript Architecture** — The application logic is split into single-responsibility modules (e.g., `showToast.js`, `removeProdFromCart.js`), keeping the codebase maintainable and easy to extend.

**Accurate Price Engine** — The cart's price calculation logic correctly handles subtotals, dynamically computed shipping fees, and tax amounts — resolving state-sync edge cases that arise when quantities change or items are removed mid-session.

**Vite for Performance** — Vite's lightning-fast Hot Module Replacement (HMR) significantly sped up the development workflow, and its optimized production builds ensure minimal bundle size for end users.

---

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to open an issue or submit a pull request.

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 👨‍💻 Author

**Ashish Kumar**

- GitHub: [@AshishKumar013](https://github.com/AshishKumar013)

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

<div align="center">
  Made with ❤️ using Vanilla JavaScript
</div>
