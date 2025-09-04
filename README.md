[README.md](https://github.com/user-attachments/files/22129836/README.md)
# product-list-app

A minimal React + Vite project that demonstrates:
- State (`useState`) holding an array of products
- Passing the product list to a `ProductList` component via props
- Mapping with `.map()` to render a `ProductItem` for each product
- Polished layout and styling via CSS
- Footer copyright: © Jose A. Hernandez Soto

## Quick Start

```bash
# Install dependencies
npm install

# Start dev server
npm run dev

# Build for production
npm run build
# Preview production build
npm run preview
```

Open the dev URL (usually http://localhost:5173) and you should see four products rendered.

## Project Structure

```
product-list-app/
├─ index.html
├─ package.json
├─ vite.config.js
└─ src/
   ├─ main.jsx
   ├─ App.jsx
   ├─ styles.css
   └─ components/
      ├─ ProductList.jsx
      └─ ProductItem.jsx
```

## Notes
- `ProductList` receives `products` as a prop and renders `<ProductItem />` for each with a unique `key`.
- `ProductItem` formats price safely with `Intl.NumberFormat` and exposes an optional `onAdd(product)`.
- Styling uses CSS variables for colors and a responsive grid layout.
