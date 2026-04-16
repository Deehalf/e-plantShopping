# Paradise Nursery

Paradise Nursery is a small e-commerce React application for browsing houseplants and managing a shopping cart. The project was built as a front-end practice app using React, Vite, and Redux Toolkit.

Users start on a landing page, move into the plant catalog, add plants to the cart, adjust quantities, remove items, and review the total amount before checkout.

This is the final project for the Coursera IBM Course about Front-End Development with React. The Github repository for this project is https://github.com/Deehalf/e-plantShopping

## Features

- Landing page with a Get Started entry point
- Product catalog grouped by plant category
- Shopping cart powered by Redux Toolkit
- Add to cart, remove item, and update quantity actions
- Automatic total cost calculation
- GitHub Pages deployment support through Vite and gh-pages

## Plant Categories

- Air Purifying Plants
- Aromatic Fragrant Plants
- Insect Repellent Plants
- Medicinal Plants
- Low Maintenance Plants

## Tech Stack

- React 18
- Vite 5
- Redux Toolkit
- React Redux
- ESLint
- GitHub Pages

## Project Structure

src/
- App.jsx: controls the landing page and product page transition
- AboutUs.jsx: introductory nursery description shown on the home screen
- ProductList.jsx: renders plant categories, plant cards, and cart access
- CartItem.jsx: renders the cart view and quantity controls
- CartSlice.jsx: Redux slice for add, remove, and quantity update actions
- store.js: Redux store configuration

## Getting Started

### Prerequisites

- Node.js 18 or newer recommended
- npm

### Installation

1. Clone the repository.
2. Open the project folder.
3. Install dependencies:

```bash
npm install
```

### Run Locally

Start the development server:

```bash
npm run dev
```

Then open the local URL shown by Vite in the terminal.

### Production Build

Create an optimized production build:

```bash
npm run build
```

Preview the production build locally:

```bash
npm run preview
```

## Available Scripts

- npm run dev: starts the Vite development server
- npm run build: creates the production build in dist
- npm run preview: serves the production build locally
- npm run lint: runs ESLint
- npm run deploy: publishes the dist folder to GitHub Pages

## Deployment Notes

This project is configured to deploy under the base path /e-plantShopping in [vite.config.js](vite.config.js).

Before deploying, make sure the repository name matches that base path or update the Vite base configuration to match your GitHub Pages repository URL.

Deployment flow:

1. Run npm run build
2. Run npm run deploy

## Current Behavior

- The cart updates item quantities and recalculates totals in real time.
- Products already added to the cart are disabled in the catalog.
- The checkout button currently shows a placeholder alert and is not connected to a payment flow.

## Learning Goals

This project demonstrates:

- Component-based UI design with React
- State management with Redux Toolkit
- Event handling and conditional rendering
- Simple cart logic for an e-commerce interface
- Basic deployment workflow with GitHub Pages

## Future Improvements

- Persist cart state in local storage
- Add product search and filtering
- Add product detail pages
- Improve accessibility and keyboard support
- Replace the checkout placeholder with a real checkout flow

## License

This repository includes a LICENSE file. Review it for usage terms.