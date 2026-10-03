# Rolsa Technologies

A responsive React website for a fictional green-energy company, built to let visitors learn about renewable energy, browse eco-friendly products, estimate their own carbon footprint, and book an installation.

**Live demo:** https://lawando69.github.io/rolsa_technologies *(update or remove this line depending on whether the GitHub Pages deployment is still live)*

## About this project

Rolsa Technologies was built as my final exam project for the T-Level in Digital Production, Design and Development at Uxbridge College. The brief was to design and build a full front-end web application within a fixed timeframe (around two and a half weeks), covering planning, UI/UX design, and implementation.

## Features

- **Home** — introduces green energy concepts (solar, EV charging, smart meters) with supporting imagery
- **Products** — a catalogue of eco-friendly energy products (solar panels, wind turbines, home energy storage, smart thermostats, and more)
- **Carbon Footprint Reduction** — an information page on practical steps for reducing personal carbon footprint
- **Calculator** — an interactive carbon footprint calculator. Takes monthly electricity/gas usage, yearly mileage and flights, and recycling habits, and returns an estimated annual footprint with a category rating (very low → exceeds limit)
- **Schedules** — a multi-step booking flow for scheduling a green energy product installation (contact details → address → product selection → confirmation)
- **Authentication** — login and registration forms (front-end only — see Known Limitations)
- **Terms & Conditions** — a full T&Cs page covering use of the calculator, bookings, payments, and liability
- Responsive design with separate desktop and mobile navigation components

## Tech stack

- [React 19](https://react.dev/) (bootstrapped with [Create React App](https://github.com/facebook/create-react-app))
- [React Router v7](https://reactrouter.com/) for client-side routing
- Plain CSS per component (no UI framework)
- Deployed via [GitHub Pages](https://pages.github.com/) (`gh-pages`)

## Getting started

Clone the repo and install dependencies:

```bash
npm install
```

Run the app in development mode:

```bash
npm start
```

Open [http://localhost:3000](http://localhost:3000) to view it in the browser. The page reloads automatically on changes.

Build a production bundle:

```bash
npm run build
```

Deploy to GitHub Pages (requires `homepage` in `package.json` to point at your own repo):

```bash
npm run deploy
```

## Project structure

```
src/
├── Assets/          # Icons and images
├── Components/       # Reusable UI components (Navbar, Footer, Logo, ProductList, WindTurbine)
├── Pages/            # One folder per route (Home, Products, CFReduction, Calculator, Schedules, Authentication, TermsConditions)
├── Pages.js          # Central route definitions
└── App.js            # App shell (navbar + routed pages + footer)
```

## Known limitations

This was a front-end-only exam project, so a few things are intentionally incomplete:

- **Authentication** has no backend — the Login/Register buttons currently just log to the console rather than creating a real session
- **Schedules** booking form collects details through a 4-step flow but doesn't submit them anywhere persistent
- **Calculator** results are rough estimates based on fixed multipliers, not a certified carbon accounting method

## Author

Lawand Salah
