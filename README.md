# Tradition Threads — Advanced GitHub Pages Website

A richer static website prototype for the **Traditional Attire for Students** project charter. Built with HTML, CSS, and vanilla JavaScript; no build step is needed.

## Features
- Editorial-style responsive design and mobile navigation
- Culture collections and cultural journal with article modals
- 10 illustrative products with product-detail modals and sample sizes
- Search, culture, occasion, price-range filters and sorting
- Saved favourites / wishlist
- Shopping bag with size selection, quantity controls, remove items and subtotal calculation
- Cart and wishlist persistence in the browser with `localStorage`
- Order enquiry and feedback email drafts
- About/story section, shopping steps, FAQ and feedback form
- Keyboard access for product detail cards, labels, reduced-motion support
- CAD currency display and clear prototype disclaimers

## Publish the update to your existing GitHub repository
Your repository is `alpeshrp23/tradition-threads`.

1. Download and unzip `tradition_threads_advanced_project.zip`.
2. Open https://github.com/alpeshrp23/tradition-threads
3. Click **Add file → Upload files**.
4. Upload the new `index.html`, `styles.css`, `script.js`, `README.md`, `.nojekyll`, and the `assets` folder (with `favicon.svg`) from this extracted project. These files should replace the older files with the same names.
5. Scroll down, enter a commit message such as `Upgrade Tradition Threads website`, and click **Commit changes**.
6. GitHub Pages should publish the new files from `main` and `/(root)`. Wait a few minutes, then refresh https://alpeshrp23.github.io/tradition-threads/ using Ctrl+F5 (Windows) or Cmd+Shift+R (Mac).

If uploading the `assets` folder is difficult, open the folder in the GitHub file upload dialog and drag its `favicon.svg` file along with the root files; preserve the `assets/favicon.svg` path. The favicon is optional, but the other four root files are required.

## Important before real sales
This remains a front-end demo. Sample products, prices, ratings, sizing, and images are illustrative, not verified supplier inventory or reviews. Some image URLs are editorial placeholders and may not depict the exact named garment. Confirm permissions and product accuracy before publishing real listings.

GitHub Pages does not run server-side code. The cart and wishlist are stored only in the visitor's browser. The order and feedback actions open an email draft using `mailto:`; no email is sent automatically and no order is stored. A blank recipient is intentional because the project charter did not provide an approved contact email. Configure the real project email or a form provider before launch.

For real commerce, connect a secure hosted checkout / store provider or backend. Do not collect card details in this static site. Add real supplier data, size charts, shipping/pickup terms, returns policy and privacy notice before accepting orders.

## Edit products
Edit `const PRODUCTS = [...]` near the top of `script.js`. Product fields include `id`, `name`, `culture`, `occasion`, `price`, `tag`, `rating`, `image`, and `description`. Keep IDs unique. Filter values must match the options in `index.html`.

## Project structure
```text
tradition_threads_advanced/
├── index.html
├── styles.css
├── script.js
├── README.md
├── .nojekyll
└── assets/
    └── favicon.svg
```
