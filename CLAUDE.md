# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a Vite-powered static website for Nurcloud, a software development company. The site is a modern, responsive single-page application showcasing the company's services, portfolio, and team.

## Development Commands

- `npm run dev` - Start development server with hot reload
- `npm run build` - Build production bundle
- `npm run preview` - Preview production build locally

## Architecture

### Tech Stack
- **Build Tool**: Vite 7.0.0
- **Frontend**: Vanilla JavaScript (ES6+)
- **Styling**: CSS with CSS custom properties (CSS variables)
- **Fonts**: Inter font family from Google Fonts
- **Icons**: Font Awesome 6.0.0

### Project Structure
```
/
├── index.html          # Main HTML file with complete site structure
├── src/
│   ├── main.js         # JavaScript for interactions and animations
│   └── styles.css      # CSS styles with custom properties
├── public/
│   └── logo.jpg        # Company logo asset
├── package.json        # Project dependencies and scripts
└── node_modules/       # Dependencies (generated)
```

### Key Features
- **Single Page Application**: All content in index.html with smooth scrolling navigation
- **Responsive Design**: Mobile-first approach with CSS Grid and Flexbox
- **Interactive Elements**: 
  - Particle animation background
  - Counter animations with Intersection Observer
  - Testimonial slider with auto-play
  - Accordion-style career listings
  - Form handling with success messages
- **Modern CSS**: Uses CSS custom properties for theming and consistent styling
- **Performance**: Preloader and optimized animations

### CSS Architecture
- CSS custom properties defined in `:root` for consistent theming
- Component-based styling approach
- Responsive design with mobile-first media queries
- Animation and transition effects throughout

### JavaScript Features
- Intersection Observer for scroll-based animations
- Smooth scrolling navigation
- Mobile menu toggle
- Form validation and submission handling
- Typewriter effect for hero title
- Particle system animation

## Development Notes

- The site uses vanilla JavaScript - no frameworks or libraries beyond Vite
- All animations use CSS transitions and JavaScript for optimal performance
- Forms are currently client-side only (no backend integration)
- Images and assets should be placed in the `public/` directory
- The site uses a dark/light theme system via CSS custom properties