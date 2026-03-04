# Pixie Petal Patch Garden Shop

A clean **React + Redux Toolkit + Vite** project that is ready for GitHub upload and GitHub Pages deployment.

## Exam-guideline coverage

### GitHub
- **Public repository URL:** create a public GitHub repository, upload this project, then paste your live repository URL into your exam submission.
- **Redux-related files/code included:**
  - `src/store.js`
  - `src/productsSlice.js`
  - `src/cartSlice.js`

### Landing page
- Background image: included in `src/App.css` on `.landing-page`
- Paragraph about the company: included on the landing page
- Company name: **Pixie Petal Patch**
- **Get Started** button: routes to the product listing page

### Product listing page
- **40 unique houseplants** are defined in `src/plantsData.js`
- Every product displays:
  - thumbnail image
  - plant name
  - price
- Plants are grouped into **4 categories**:
  - Tropical Foliage
  - Flowering Beauties
  - Easy-Care Favorites
  - Trailing & Hanging

### Extra shopping-cart features (added to help with common rubric items)
- Add to Cart button on each product
- Cart item count in the header
- Separate cart page
- Increase quantity
- Decrease quantity
- Remove item
- Clear cart
- Total item count and total cost

## Run locally

```bash
npm install
npm run dev
```

Then open the local Vite URL shown in the terminal.

## Build locally

```bash
npm run build
npm run preview
```

## Upload to GitHub

1. Create a **public** GitHub repository.
2. Upload all project files from this folder.
3. Commit to the `main` branch.
4. Push the project.

## Publish on GitHub Pages

This project already includes:
- `vite.config.js` with `base: './'`
- `.github/workflows/deploy.yml`

To publish:
1. Push the project to GitHub.
2. Open the repository on GitHub.
3. Go to **Settings → Pages**.
4. Under **Build and deployment**, set **Source** to **GitHub Actions**.
5. Push to `main` again if needed.

The workflow will build the app and deploy the `dist` folder automatically.


## Install notes

This project includes a project-level `.npmrc` that points to the public npm registry so `npm install` and `npm ci` work on a normal local machine and on GitHub Actions.

If you ever see a timeout to a non-public registry URL, delete `node_modules`, then run:

```bash
npm cache clean --force
npm ci
```
