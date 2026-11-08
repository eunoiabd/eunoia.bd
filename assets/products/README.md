# Product photos

Put every new product photo in this folder (`assets/products/`).

- Format: `.jpg` or `.png`
- Square photos look best (the cards crop to a fixed box)
- Small file names, no spaces — e.g. `oversized-tee.jpg`

Then list each photo in `index.html`, inside the `const products=[ ... ]` block:

```js
const products=[
  {name:'Oversized Tee',img:'assets/products/oversized-tee.jpg',price:'৳ 990'},
  {name:'Cargo Pants',img:'assets/products/cargo.jpg',price:'৳ 1,450',sizes:['30','32','34'],colors:['Black','Olive']},
];
```

- Newest product goes **last** — the last two are shown under "OUR NEWEST PRODUCTS".
- `sizes` and `colors` are optional; without them the site uses S/M/L/XL and Black/White/Olive.
- `imgs:['a.jpg','b.jpg',...]` is optional: extra photos shown as thumbnails in the product popup. The main `img` should be the first one (it is also the card photo).
- An empty list (`const products=[]`) shows the "New collection coming soon" message.
