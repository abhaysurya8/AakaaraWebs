# Aakaara Architecture Website

A professional architecture and interior design website recreated to match the exact design from your HTML template, featuring Montserrat and Playfair Display fonts, brown sidebar design, and responsive layout.

## Features

- ✅ Exact layout matching your HTML design
- ✅ Montserrat font for body text, Playfair Display for headings
- ✅ Brown sidebar with vertical "aakaara" text
- ✅ Hamburger menu icon (top-left)
- ✅ Multi-page navigation (Home, About, Projects, Pricing, Contact)
- ✅ Pricing comparison table between Elegance and Elite packages
- ✅ Contact form with validation
- ✅ Back to top button
- ✅ Mobile responsive design
- ✅ Easy font customization setup

## Complete Setup Instructions

### 1. Install Node.js (if not already installed)
Download and install Node.js from https://nodejs.org/

### 2. Install Dependencies
```bash
npm install
```

### 3. Add Your Rigot Bold Font
1. Create the fonts directory:
   ```bash
   mkdir -p client/public/fonts
   ```

2. Place your Rigot Bold font files in `client/public/fonts/`:
   - `Rigot-Bold.woff2` (recommended)
   - `Rigot-Bold.woff` (fallback)
   - `Rigot-Bold.ttf` (fallback)

   The CSS will automatically detect and use your font for the "aakaara" branding.

### 4. Start the Development Server
```bash
npm run dev
```

The website will be available at `http://localhost:5000`

### 5. Build for Production (when ready to deploy)
```bash
npm run build
```

## Project Structure

```
client/
├── public/
│   └── fonts/           # Place your Rigot Bold font files here
├── src/
│   ├── components/
│   │   ├── Layout.tsx   # Hamburger menu, navigation, footer
│   │   └── BackToTop.tsx # Back to top button
│   ├── pages/
│   │   ├── Home.tsx     # Main landing page with brown sidebar
│   │   ├── About.tsx    # "Crafting Inspired Spaces" with photo
│   │   ├── Projects.tsx # Portfolio showcase
│   │   ├── Pricing.tsx  # Elegance vs Elite comparison table
│   │   └── Contact.tsx  # Contact form
│   └── index.css        # Fonts and styling
server/
├── index.ts            # Express server
└── routes.ts           # API endpoints
```

## Design System

### Typography
- **Body Text**: Montserrat (Google Fonts)
- **Headings**: Playfair Display (Google Fonts)
- **Brand "aakaara"**: Rigot Bold (your custom font) or Playfair Display fallback

### Colors (matching your design)
- **Text Color**: #7f6a4d (brown text)
- **Sidebar Background**: #5a3a22 (dark brown)
- **Sidebar Text**: #d9c4b0 (light brown)
- **Background**: #ffffff (white)

### Layout
- **Home Page**: Two-column layout with brown sidebar containing vertical "aakaara" text
- **Navigation**: Architecture, Interior, Landscape links in sidebar
- **Footer**: Brown background with contact information
- **Menu**: Hamburger icon (top-left) for mobile/overlay navigation

## Pages

### Home Page (`/`)
Exact recreation of your HTML design:
- Main content area with services description
- Brown sidebar (220px width) with navigation links
- Vertical "aakaara" text in Rigot Bold (bottom-right of sidebar)

### About Page (`/about`)
- "Crafting Inspired Spaces" title
- Circular architect photo
- Company description

### Pricing Page (`/pricing`)
- Professional table comparing Elegance (₹1,779) vs Elite (₹2,249)
- All features listed exactly as specified
- Checkmarks and detailed descriptions

### Contact Page (`/contact`)
- Contact form with validation
- Professional layout

### Projects Page (`/projects`)
- Portfolio grid layout
- Sample project showcase

## Font Customization

The website is set up to easily use your Rigot Bold font:

1. **If you have Rigot Bold**: Place font files in `client/public/fonts/`
2. **If you don't have it**: The design will use Playfair Display as fallback

Supported font formats: .woff2, .woff, .ttf, .otf

## Development Stack

- **Frontend**: React + TypeScript + Vite
- **Styling**: Tailwind CSS + Google Fonts
- **Backend**: Express.js + TypeScript
- **Routing**: Wouter (client-side)

## Running the Project

1. Clone/download the project
2. Run `npm install`
3. Add your font files (optional)
4. Run `npm run dev`
5. Open `http://localhost:5000`

The website now matches your exact HTML design with proper React architecture and full functionality!