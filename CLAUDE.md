# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a Shopify e-commerce project inspired by Nike.com, designed to create a high-end fashion/sportswear store using Shopify's platform. The project focuses on replicating Nike's modern design, user experience, and functionality.

## Current State

- **Repository Status**: Active development - Basic theme structure complete
- **Primary Language**: Liquid (Shopify's templating language), HTML, CSS, JavaScript
- **Framework/Platform**: Shopify Online Store 2.0 with custom theme development
- **Development Stage**: Week 2-3 - Homepage & Navigation phase
- **Branch**: main

### Completed Components
- ✅ Base theme layout (`layout/theme.liquid`)
- ✅ Responsive header with navigation (`sections/header.liquid`)
- ✅ Dropdown menu system with Alpine.js
- ✅ Shopping cart icon (`snippets/icon-shopping-bag.liquid`)
- ✅ Dropdown icon (`snippets/icon-dropdown.liquid`)
- ✅ Tailwind CSS v4.1.16 integration
- ✅ Alpine.js integration for interactivity

### In Progress
- 🚧 Homepage hero section
- 🚧 Product grid layouts
- 🚧 Mobile navigation menu

### Pending
- ⏳ Footer section
- ⏳ Product page templates
- ⏳ Collection pages
- ⏳ Cart functionality
- ⏳ Search functionality
- ⏳ Customer account pages

## Technical Stack

- **Shopify CLI**: For theme development and deployment
- **Liquid**: Shopify's templating language
- **HTML5/CSS3**: Modern web standards
- **Tailwind CSS v4.1.16**: Utility-first CSS framework (installed)
- **Alpine.js v3**: Lightweight JavaScript framework for interactivity (integrated)
- **JavaScript (ES6+)**: Interactive features and dynamic content
- **Dawn Theme**: As base reference (Shopify's official theme)

## Key Features to Implement

### Core Nike.com Features
- Responsive grid-based product layouts
- Dynamic carousel components  
- Advanced product filtering and search
- Product customization options
- Mega menu navigation
- Video backgrounds and animations
- Mobile-first responsive design
- Performance optimization

### Shopify-Specific Features
- Online Store 2.0 block architecture
- Shopify Checkout integration
- Inventory management
- Multi-language support
- SEO optimization
- Analytics integration

## Development Workflow

### Commands
```bash
# Install Shopify CLI
npm install -g @shopify/cli @shopify/theme

# Create new theme from Dawn
shopify theme init

# Start development server
shopify theme dev

# Deploy to store
shopify theme push
```

### Project Structure
```
/
├── assets/          # CSS, JS, images
├── config/          # Theme settings
├── layout/          # Base templates
├── locales/         # Translation files
├── sections/        # Reusable components
├── snippets/        # Partial templates
├── templates/       # Page templates
└── package.json     # Dependencies
```

## Architecture

The project follows Shopify Online Store 2.0 architecture with:
- Modular section-based design
- JSON templates for flexibility
- Reusable snippets and components
- Block-based content management
- Performance-optimized asset loading

## Development Phases

1. **Setup & Environment** (Week 1) ✅ COMPLETED
   - Tailwind CSS installed
   - Alpine.js integrated
   - Base file structure created

2. **Basic Theme Structure** (Week 2) ✅ COMPLETED
   - Theme layout created
   - Header section with navigation built
   - Icon snippets created

3. **Homepage & Navigation** (Week 3-4) 🚧 IN PROGRESS
   - ✅ Desktop navigation with dropdowns
   - ⏳ Mobile menu
   - ⏳ Hero section
   - ⏳ Featured products grid

4. **Product Pages & Collections** (Week 5-6) ⏳ PENDING
5. **Cart & Checkout Enhancement** (Week 7) ⏳ PENDING
6. **Performance & SEO** (Week 8) ⏳ PENDING
7. **Testing & Launch** (Week 9) ⏳ PENDING