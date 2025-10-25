# React + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react) uses [Babel](https://babeljs.io/) (or [oxc](https://oxc.rs) when used in [rolldown-vite](https://vite.dev/guide/rolldown)) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

## React Compiler

The React Compiler is not enabled on this template because of its impact on dev & build performances. To add it, see [this documentation](https://react.dev/learn/react-compiler/installation).

## Expanding the ESLint configuration

If you are developing a production application, we recommend using TypeScript with type-aware lint rules enabled. Check out the [TS template](https://github.com/vitejs/vite/tree/main/packages/create-vite/template-react-ts) for information on how to integrate TypeScript and [`typescript-eslint`](https://typescript-eslint.io) in your project.

## code structure

e-commerce/
├── public/
│ └── index.html
├── src/
│ ├── assets/ # Images, icons, fonts
│ ├── components/ # Reusable UI components
│ │ ├── Navbar.jsx
│ │ ├── Footer.jsx
│ │ ├── ProductCard.jsx
│ │ ├── CartItem.jsx
│ │ └── ...
│ ├── pages/ # Route-based pages
│ │ ├── Home.jsx
│ │ ├── Products.jsx
│ │ ├── ProductDetails.jsx
│ │ ├── Cart.jsx
│ │ ├── Wishlist.jsx
│ │ ├── Checkout.jsx
│ │ ├── Login.jsx
│ │ ├── Signup.jsx
│ │ ├── Dashboard.jsx # Admin dashboard
│ │ └── ...
│ ├── features/ # Redux slices or context modules
│ │ ├── auth/
│ │ ├── cart/
│ │ ├── products/
│ │ ├── orders/
│ │ └── ...
│ ├── hooks/ # Custom React hooks
│ │ └── useAuth.js
│ ├── layouts/ # Page layouts (e.g., AdminLayout, MainLayout)
│ ├── routes/ # Route definitions
│ │ └── AppRoutes.jsx
│ ├── services/ # Firebase, Axios, Stripe, etc.
│ │ ├── firebase.js
│ │ ├── api.js
│ │ └── stripe.js
│ ├── styles/ # Global styles or Tailwind config
│ │ └── tailwind.css
│ ├── utils/ # Helper functions
│ │ └── formatCurrency.js
│ ├── App.jsx
│ ├── index.js
│ └── .env.local # Environment variables
├── .gitignore
├── package.json
└── README.md
