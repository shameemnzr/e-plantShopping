# Paradise Nursery Shopping Application

Paradise Nursery is a responsive, feature-rich React web application designed for plant enthusiasts to browse and purchase a wide variety of houseplants. Built with React and Redux Toolkit, this application provides a seamless and interactive user shopping experience across multiple pages.

## Deployed Application
You can view the live deployment of the application here:  
👉 **[Live Demo on GitHub Pages](https://shameemnzr.github.io/e-plantShopping/)** 

---

## Features

### 1. Landing Page
- **Immersive Visuals:** Features a beautiful nature-inspired background image welcoming users.
- **Company Profile:** Includes an engaging overview paragraph introducing Paradise Nursery's mission.
- **Call to Action:** A dedicated **"Get Started"** button that smoothly guides users directly to the product catalog.

### 2. Product Listing Page
- **Diverse Catalog:** Features at least six unique houseplants organized neatly into three or more distinct categories.
- **Detailed Product Cards:** Each item displays a thumbnail image, plant name, and price.
- **Dynamic Cart Interactions:** 
  - Clicking the **"Add to Cart"** button adds the item to the persistent global state.
  - The button instantly updates to **"Added"** and becomes disabled to prevent duplicate selections from the catalog.

### 3. Shared Navigation Header
- **Persistent Navbar:** Available on both the Product Listing and Shopping Cart pages.
- **Dynamic Cart Badge:** Displays a shopping cart icon with a real-time badge counting the total number of items currently in the cart.
- **Smooth Navigation:** Allows instant switching between the Home landing page, Plant catalog, and the Shopping Cart.

### 4. Shopping Cart Page
- **Order Summary:** Displays the total number of plants and the breakdown of costs, including individual item unit prices and subtotals.
- **Quantity Controls:** Includes intuitive `+` and `-` buttons to modify plant quantities dynamically.
- **Item Removal:** A dedicated delete button is provided to remove specific plant types from the cart entirely.
- **Intuitive Workflows:**
  - A **"Continue Shopping"** button easily routes users back to the plant listing page.
  - A **"Checkout"** button provides feedback with a "Coming Soon" notification.

---

## Tech Stack & Architecture

- **Frontend Framework:** React (Functional Components & Hooks)
- **State Management:** Redux Toolkit (`@reduxjs/toolkit` and `react-redux`)
  - Utilizing a centralized `CartSlice.jsx` to maintain cart state, track quantities, and update global totals dynamically.
- **Styling:** CSS3 (`App.css` for background layouts and global styling)
- **Deployment:** GitHub Pages

---

## File Structure Highlights

```text
├── src/
│   ├── components/
│   │   ├── AboutUs.jsx       # Component detailing the company profile
│   │   ├── ProductList.jsx   # Grid catalog displaying plants by category
│   │   └── CartItem.jsx      # Shopping cart view with quantity management
│   ├── store/
│   │   └── CartSlice.jsx     # Redux slice managing actions (addItem, removeItem, updateQuantity)
│   ├── App.jsx               # App entry point, routing, and Landing Page layout
│   ├── App.css               # Background imagery and layout styling
│   └── main.jsx
├── public/
├── package.json
└── README.md
