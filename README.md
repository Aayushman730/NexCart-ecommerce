# NexCart-ecommerce
A responsive e-commerce website built using HTML, CSS, JavaScript, and **DummyJSON API**.It allows users to browse products, search items, view product details, and manage their shopping cart using localStorage.


## ✨ Features
🔍 Live Product Search — Instantly filter products as you type
🛍️ Product Listing — Browse 194+ products fetched from DummyJSON API
📄 Product Details Page — View full product info including description and price
🛒 Shopping Cart — Add and remove products with a persistent cart using localStorage
💰 INR Pricing — Prices dynamically converted from USD to Indian Rupees (₹)
📱 Fully Responsive — Optimized for mobile, tablet, and desktop screens


## 🗂️ Project Structure

```text
NexCart-ecommerce/
├── index.html       # Home page — product listing
├── product.html     # Product details page
├── cart.html        # Shopping cart page
├── app.js           # Product listing & search logic
├── product.js       # Product details & add-to-cart logic
├── cart.js          # Cart display & remove item logic
├── style.css        # Global styles & responsive design
└── README.md
```


## 🛠 Tech Stack
| Technology | Usage |
|------------|-------|
| HTML5 | Page structure |
| CSS3 | Styling & Responsive Layout |
| JavaScript (ES6+) | Dynamic rendering, DOM manipulation, API calls |
| LocalStorage | Store cart items locally |
| DummyJSON API | Product data source |


## 🚀 Getting Started

No installation or build tools needed — this is a pure frontend project.

### 1. Clone the repository

```bash
git clone https://github.com/Aayushman730/NexCart-ecommerce.git
cd NexCart-ecommerce
```

### 2. Open in browser

Simply open `index.html` in your browser.

```bash
# Option 1: Double-click index.html

# Option 2: Use VS Code Live Server extension

# Option 3: Use a local server
npx serve .
```


## 📖 How It Works

### 🏠 Home Page (`index.html` + `app.js`)

- Fetches 194 products from https://dummyjson.com/products
- Displays them in a responsive grid of cards
- Search bar filters products in real-time by title

### 📄 Product Page (`product.html` + `product.js`)

- Reads the product id from the URL query string
- Fetches that specific product from the API
- Displays the image, title, description, and INR price
- "Add to Cart" button saves the product to localStorage

### 🛒 Cart Page (`cart.html` + `cart.js`)

- Reads saved cart items from localStorage
- Displays each item with its image, name, and price
- Calculates and shows the total bill
- "Remove" button deletes individual items from the cart


## 🔗 API Reference

This project uses the free **DummyJSON API**.

| Endpoint | Description |
|----------|-------------|
| `GET /products?limit=194` | Fetch all products |
| `GET /products/:id` | Fetch a single product by ID |


## 📱 Responsive Breakpoints

| Breakpoint | Layout |
|------------|--------|
| `> 992px` | 3+ column product grid |
| `768 - 992px` | 2 column product grid |
| `<= 768px` | 1 column, stacked navbar |
| `<= 576` | Single column layout |


## 🤝 Contributing

Contributions are welcome! Feel free to:

1. Fork the repository
2. Create a new branch (`git checkout -b feature/your-feature`)
3. Commit your changes (`git commit -m "Add some feature"`)
4. Push to the branch (`git push origin feature/your-feature`)
5. Open a Pull Request

## 📄 License

This project is open source and available under the **MIT License**.

## 👤 Author

**Aayushman Khare**

- GitHub: [@Aayushman730](https://github.com/Aayushman730)
