# :shopping_trolley: MERN E-Commerce Frontend (React)

This is the *frontend* part of a full-stack MERN (MongoDB, Express.js, React, Node.js) E-Commerce application. The React application includes both *user-facing* and *admin-facing* components, with full functionality for browsing products, user authentication, cart, checkout, order management, and administrative controls.

---

## :spanner: Tech Stack

- *React.js* – Frontend framework
- *React Router* – Client-side routing
- *Axios* – HTTP client for API requests
- *Redux / Context API* – (If applicable, for state management)
- *Bootstrap / Tailwind / Material UI* – (If applicable, for UI components)

---

## :file_folder: Component Structure

### :silhouette: User Components

- Register.jsx – User registration form
- Login.jsx – User login form
- Profile.jsx – View and edit user profile
- GetAllUser.jsx – Admin view to manage all users

### :shopping_bags: Product Components

- ShowProduct.jsx – Display all products to users
- ProductDetail.jsx – Single product detailed view
- RelatedProduct.jsx – Show related products based on category
- SearchProduct.jsx – Product search functionality
- AddProduct.jsx – Admin interface to add a new product
- EditProduct.jsx – Admin interface to edit existing product
- ShowProductAdmin.jsx – Admin panel to view all products

### :shopping_trolley: Cart & Checkout

- Cart.jsx – Shopping cart view
- Address.jsx – Shipping address input
- Checkout.jsx – Checkout and payment process
- OrderConfirmation.jsx – Confirmation after successful order

### :package: Orders (Admin)

- AllOrder.jsx – Admin view to manage and track all orders

### :link: Other Components

- Navbar.jsx – Top navigation bar (responsive & role-aware)

---

## ★ MERN E-Commerce API

### :silhouette: User API Endpoints

- POST - /api/user/register – Register a new user
- POST - /api/user/login – Login existing user
- GET - /api/user/profile – Get user profile (*Auth required*)
- GET - /api/user/all – Get all users (Admin only)

### :package: Product API Endpoints

- POST - /api/product/add – Create a new product
- GET - /api/product/all – Retrieve all products
- GET - /api/product/:id – Get a specific product by ID
- PUT - /api/product/:id – Update a product by ID
- DELETE - /api/product/:id – Delete a product by ID

### :shopping_trolley: Cart API Endpoints

- POST - /api/cart/add – Add a product to the cart (*Auth required*)
- GET - /api/cart/user – Retrieve the user's cart (*Auth required*)
- POST - /api/cart/--qty – Decrease quantity of a product in the cart (*Auth required*)
- DELETE - /api/cart/remove/:productid – Remove a product from the cart (*Auth required*)
- DELETE - /api/cart/clear – Clear all products from the cart (*Auth required*)

### :house: Shipping Address API Endpoints

- POST - /api/address/add – Add shipping address (*Auth required*)
- GET - /api/address/get – Get shipping address (*Auth required*)

### :credit_card: Payment API Endpoints

- POST - /api/payment/checkout – Initiate the payment process
- POST - /api/payment/verify-payment – Confirm payment and save order

### :white_tick: Order Confirmation API Endpoints

- GET - /api/order/confirm – Get user-specific orders (*Auth required*)
- GET - /api/order/confirm/all – Get all users' orders (Admin only)

---

## :rocket: Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/devyanshidubey-02/MERN_E-COMMERCE.git
cd mern-ecommerce-frontend