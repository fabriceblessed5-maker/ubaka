# UBAKA.com – React front end

## Run
    npm install
    npm run dev

## Routes
| Path            | Page                                   |
|-----------------|----------------------------------------|
| `/`             | Home                                   |
| `/products`     | Catalogue (search, filters, sort, pages); `?cat=amazi` etc. preselects a category |
| `/cart`         | Cart with live totals and payment picker |
| `/login`        | Customer login (full screen)           |
| `/admin/login`  | Admin login (full screen)              |

## Images
Copy your images into `public/images/`:
elepic1.png, elepic2.png, elepica1.png, elepicb2.png, plum1.png, plum1.jpeg, plumb.png,
pluming.jpeg, cons1.jpeg, cons2.png, construction.jpeg, clays.jpg, bricks.jpeg, bricks.png,
toolkits.png, biglines.png, logo.jpg

## Structure
- `src/data/`        site config, categories, products, banners, payments
- `src/context/`     CartProvider (reducer + localStorage)
- `src/hooks/`       useCart, useProductCatalog, useForm, usePageTitle
- `src/services/`    authService (placeholder API calls)
- `src/utils/`       formatting helpers
- `src/components/`  layout, home, products, cart, auth, common
- `src/pages/`       Home, Products, Cart, Login, AdminLogin, NotFound
- `src/styles/`      base, layout, home, products, cart, auth, responsive

## Notes
- The cart starts with the three demo items from your cart page. Set `SEED_CART` to `[]` in
  `src/context/CartProvider.jsx` for an empty start.
- Add new products in `src/data/products.js`; the grid, filters and cart pick them up automatically.
