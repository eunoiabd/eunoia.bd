# eunoia.bd
An e-commerce website and inventory management system for RELOVED clothing shop.

## Adding products

All products live in one list inside `index.html` — search for `const products=[`.
Photos go in `assets/products/` (see the README in that folder).

```js
const products=[
  {name:'Oversized Tee',img:'assets/products/oversized-tee.jpg',price:'৳ 990'},
  {name:'Cargo Pants',img:'assets/products/cargo.jpg',price:'৳ 1,450',sizes:['30','32','34'],colors:['Black','Olive']},
];
```

- Newest product goes **last** — the last two are shown automatically under "OUR NEWEST PRODUCTS", and the last one becomes the hero photo.
- `sizes` / `colors` are optional (defaults: S–XL, Black/White/Olive).
- The list is currently empty, so the site shows a "New collection coming soon" panel with a WhatsApp button instead of an empty grid.

## Preview locally

```bash
python3 -m http.server 8000 --bind 0.0.0.0
```

Then open http://localhost:8000
