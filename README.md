# RecipeNest — React + Vite

A responsive recipe discovery website built with React and Vite. It includes a user-facing recipe library, search and category filters, recipe detail views, favourites, localStorage-based login/signup, and an Admin Studio for adding and removing recipes.

## Run locally

1. Install Node.js (LTS).
2. Open this folder in VS Code.
3. Open the terminal and run:

```bash
npm install
npm run dev
```

4. Open the local URL printed by Vite (usually `http://localhost:5173`).

## Build for deployment

```bash
npm run build
npm run preview
```

Vite outputs the production site to `dist/`.

## Login and Admin module

- Sign up with your name, email and password, then log in on later visits.
- To open Admin Studio, create an account with the exact email `admin@recipenest.com`. For this classroom demo, the app assigns the admin role based on that email.
- Admin Studio can publish new recipes. Admin users can also remove recipes from the recipe cards.
- Regular users can browse recipes and save favourites.

## Data and security note

This is a front-end academic demonstration. Accounts, session, favourites and recipes are stored in the browser's `localStorage`. Passwords are therefore **not secure** and data is browser/device-specific. Do not use real or reused passwords. A production app should use a backend and secure authentication. The seeded recipe data returns if localStorage is cleared.

## Deploy to Vercel

1. Create a GitHub repository and upload/push the contents of this folder (the `src` folder, `index.html`, `package.json`, etc.). Do not upload `node_modules`.
2. In Vercel, choose **Add New → Project**, import the GitHub repository, and deploy.
3. Vercel should detect Vite automatically. Build command: `npm run build`; output directory: `dist`.
4. Open the deployed URL and test signup, login, category filtering, search, favourites and Admin Studio.

## Suggested review demonstration

1. Show the responsive homepage and recipe cards.
2. Search for “pasta” and switch recipe categories.
3. Open a recipe and explain the ingredients and steps.
4. Create a normal user account and save a favourite.
5. Sign out, create/log in with `admin@recipenest.com`, open **Admin Studio**, add a recipe, then show it in the library.
6. Refresh the page to demonstrate localStorage persistence.
7. Show the GitHub repository and deployed Vercel link.
