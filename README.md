# Elizabeth Clean Shopify Theme

A Shopify Online Store 2.0 starter theme built for the [Shopify Theme Development – Online Store 2.0 + TailwindCSS](https://weeklyhow.com/courses/) course. It ships with Tailwind CSS v4, Alpine.js-powered navigation, and ready-to-edit templates for every core storefront page so you can focus on customizing the experience for your brand.

## Highlights
- Shopify OS 2.0 structure with JSON sections, reusable snippets, and language-ready locales
- Tailwind CSS v4 workflow compiled from `src/tailwind.css` into `assets/application.css`
- Alpine.js-enhanced responsive header with dropdown menus and cart shortcut
- Coverage for homepage, collections, products, blog/article, search, 404, cart, and customer account flows
- Minimal JavaScript (`assets/application.js`) and lightweight CSS output so you can layer in features as you go

## Project Structure
```
assets/                 # Compiled theme assets (Tailwind build, logo, app JS)
config/                 # Theme settings schema and presets
layout/theme.liquid     # Global HTML wrapper, loads header section and assets
locales/                # Translation strings (defaults provided by Shopify)
sections/               # Header and homepage sections (add new sections here)
snippets/               # Reusable fragments (icons, homepage text)
src/tailwind.css        # Tailwind CSS source entry point
templates/              # Liquid templates for all core Shopify resources
```

## Requirements
- Node.js 18+ (needed for the Tailwind CLI)
- Shopify CLI (`npm install -g @shopify/cli` or follow the [official guide](https://shopify.dev/themes/tools/cli/installation))
- Access to a Shopify development store with a staff or collaborator account

## Getting Started
1. **Install dependencies**
   ```sh
   npm install
   ```
2. **Compile Tailwind CSS during development**
   ```sh
   npx tailwindcss -i src/tailwind.css -o assets/application.css --watch
   ```
3. **Run the Shopify local development server**
   ```sh
   shopify theme dev --store <your-development-store>
   ```
   The CLI pushes theme changes to your development store and provides a preview URL. Modify Liquid templates/sections and Tailwind source files to see updates live.

## Building for Release
Generate a production CSS bundle and push the theme to your store:
```sh
npx tailwindcss -i src/tailwind.css -o assets/application.css --minify
shopify theme push --store <your-development-store>
```

## Customization Notes
- **Navigation**: The header reads from the `main-menu-1` navigation. Nested menu items automatically render as dropdowns via Alpine.js.
- **Homepage**: `templates/index.liquid` loads the `sections/homepage.liquid` section; customize layout by editing or adding sections.
- **Typography & spacing**: Adjust Tailwind utility tokens in `assets/application.css` by editing the source `src/tailwind.css` and rebuilding.
- **Snippets**: Reuse Liquid fragments in `snippets/` (icons, homepage copy) to keep templates clean.
- **Localization**: Update storefront copy through the files in `locales/` or via the Shopify admin language editor.

## Course Context & Support
This repository mirrors the theme built in the WeeklyHow course. Questions about the course material are handled via the course Q&A. If you're using this theme outside the course, you're welcome to extend it, but community support is limited.

Happy theming!
