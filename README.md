# TechBlog

A modern, responsive blog focused on web development, design, and technology. Built with clean HTML and CSS, featuring a focus on accessibility and user experience.

## Features

- Responsive design that works on desktop, tablet, and mobile
- Accessible focus indicators with pulsing animations
- Semantic HTML structure for better SEO and screen readers

## HTML Structure

The HTML is structured semantically for clarity and accessibility:

- **`<header>`**: Contains the site logo, navigation menu, and subscribe button
- **`<section>` (Hero)**: Welcome message and search input
- **`<main>`**: Contains the featured articles section
  - **`<section aria-label="Featured Articles">`**: List of blog posts with images, categories, dates, and excerpts
- **`<aside>`**: Sidebar with categories, popular posts, and newsletter signup
  - **`<section aria-label="Categories">`**: List of article categories
  - **`<section aria-label="Popular posts">`**: Thumbnails and links to popular articles
  - **`<section aria-label="Newsletter">`**: Email signup form
- **`<footer>`**: Site footer with links, contact info, and social media icons

Key accessibility features:
- ARIA labels for sections
- Semantic headings (h1-h4)
- Alt text on images
- Proper form labels and placeholders

## CSS Structure

The CSS uses CSS custom properties (variables) for maintainability and a nested structure for organization.

### Variables (`:root`)

- **Colors**: Base colors like `--color-accent`, `--color-text-primary`, etc., with derived variables for specific elements
- **Spacing**: `--padding-section`, `--gap-large`, etc.
- **Icons**: URLs for SVG icons from Icônes (Iconify)
- **Other**: Border radius, font family, etc.

### Key Selectors

- **Global**: `:focus-visible` for accessible focus outlines with pulsing animation
- **Header**: Flexbox layout for logo, nav, and button
- **Hero**: Gradient background, centered content
- **Articles**: Card-like layout with images, pills for categories, and hover effects
- **Sidebar**: Sections for categories, posts, and newsletter with distinct styling
- **Footer**: Multi-column layout with social icons
- **Responsive**: Media queries for tablet and mobile breakpoints

### Animations

- `borderPulse`: Fades the focus outline for visual feedback
- Applied to focusable elements with `animation: borderPulse .75s infinite alternate;`

### Responsive Design

- Desktop: Full layout with sidebar
- Tablet (1280px): Adjusted padding and flex direction
- Mobile (820px): Stacked layout, reduced padding

## Technologies Used

- HTML5
- CSS3
- Icônes (Iconify) for icons
- Inter font from Google Fonts