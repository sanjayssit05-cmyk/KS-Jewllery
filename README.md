# KS Jewllerys Jewellery

A responsive multi-page jewellery storefront built with semantic HTML, CSS and vanilla JavaScript. The catalogue and interactions are frontend demo content; there is no backend or payment processing.

## Project files

```text
index.html          Home page
shop.html           Searchable, filterable catalogue
product.html        Product details (select a product from the shop)
wishlist.html       Saved favourites
cart.html            Shopping bag
checkout.html        Validated demo checkout
about.html           Brand story
contact.html         Contact demo and FAQ
privacy.html         Demo privacy notice
terms.html           Demo terms notice
404.html             Custom not-found page
style.css            Shared responsive design system
products.js          Twenty illustrative product records
script.js            Shared page rendering and storefront behaviour
README.md            Setup and production notes
```

## Run locally

Open `index.html` directly in a browser, or serve the folder with any static HTTP server. For example, with Python installed, run `python -m http.server 8000` in this folder and visit `http://localhost:8000`. All pages share `style.css`, `products.js` and `script.js`.

## Try the demo

- Browse `shop.html`; combine category, price and text search, change sorting, and load more products.
- Open a product for gallery, size selection, quantity, quick view and related items.
- Save favourites and add items to the bag. Both are stored in this browser's local storage.
- Change item quantities, remove items and continue to checkout. Shipping is complimentary over ₹10,000; otherwise this demo uses a ₹450 fee.
- Submit the checkout or contact forms to see the demo confirmation. The checkout does not accept card details and does not submit an order. Newsletter and contact forms do not send data.
- Use the theme, global search, FAQ, and mobile navigation controls.

Product prices, ratings, review counts, stock, materials, contact details, shipping and policy language are illustrative. Unsplash image URLs require an internet connection and include a fallback image if loading fails.

## Publish as a static site

1. Create a Git repository in this folder, then run `git add .`, `git commit -m "Build KS Jewllerys jewellery storefront"`, and `git push` to your GitHub repository.
2. In Vercel, import that repository and deploy it as a static site. No build command is needed; use `.` as the output directory if prompted.
3. Verify page links and forms on the deployed domain. All HTML pages must be included in the deployment.

## What production would need

A real business needs a secure backend/API, a product catalogue database, authenticated customer accounts (if offered), inventory and fulfilment integrations, order management, transactional email, and a payment provider with server-side verification, webhooks and appropriate compliance. Add real shipping, tax, returns and privacy policies for the operating jurisdictions. Never handle raw card data in frontend JavaScript. Replace all sample catalogue, review, price, availability and contact data before launch.
