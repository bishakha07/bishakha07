# Creative Developer Portfolio 🚀

A modern, vibrant, and highly animated portfolio built with Next.js 16, React 19, Tailwind CSS, and Framer Motion. Showcasing AI/ML expertise, full-stack development, and blockchain projects with a bold neon color palette and smooth animations.

## Features

### Design & Aesthetics
- **Vibrant Color Palette**: Hot pink (#ff1493), cyan (#00d4ff), neon green (#00ff88), orange (#ffa502), and purple (#9d4edd) with dark navy background
- **Glassmorphism Effects**: Frosted glass cards with backdrop blur and transparency
- **Smooth Animations**: Staggered entrances, scroll triggers, hover effects, and floating background orbs
- **Fully Responsive**: Mobile-first design that works seamlessly on all devices

### Content Sections
1. **Navigation Bar** - Fixed navbar with animated underlines and glowing logo
2. **Hero Section** - Eye-catching intro with animated text reveal and gradient CTA buttons
3. **Experience** - AI internship details with key highlights and technologies
4. **Education** - University background, specialization, and 11+ professional certifications
5. **Projects** - 6 showcase projects (AI/ML, Frontend, Full-Stack, Blockchain) with gradient cards and color-coded badges
6. **Skills** - 6+ skill categories with progress bars and interactive tech tags
7. **Impact** - Key achievements and career stats
8. **Contact** - Call-to-action section with email and social media links

### Interactive Elements
- **Scroll Progress Bar** - Visual indicator of page scroll progress
- **Back-to-Top Button** - Smooth scroll to top on click
- **Hover Animations** - Interactive hover effects on buttons, cards, and links
- **Floating Background** - Animated gradient orbs that move subtly in the background
- **Neon Glow Effects** - Glowing borders and shadows on interactive elements

## Tech Stack

- **Framework**: Next.js 16 (App Router)
- **React**: React 19 with latest features
- **Styling**: Tailwind CSS 4.2 with custom design tokens
- **Animations**: Framer Motion for smooth, performant animations
- **Icons**: Lucide React
- **Fonts**: Google Fonts (Geist)
- **Build Tool**: Turbopack (default in Next.js 16)

## Project Structure

```
├── app/
│   ├── layout.tsx           # Root layout with dark mode enabled
│   ├── page.tsx             # Main portfolio page
│   └── globals.css          # Global styles with design tokens and animations
├── components/
│   ├── sections/            # Main content sections
│   │   ├── navbar.tsx       # Navigation bar
│   │   ├── hero.tsx         # Hero introduction
│   │   ├── experience.tsx   # Work experience
│   │   ├── education.tsx    # Education & certifications
│   │   ├── projects.tsx     # Project showcase
│   │   ├── skills.tsx       # Skills & proficiencies
│   │   ├── impact.tsx       # Impact/achievements
│   │   └── contact.tsx      # Contact & social links
│   ├── animation-wrapper.tsx # Reusable animation component
│   ├── floating-background.tsx # Animated background orbs
│   ├── scroll-progress.tsx  # Scroll progress indicator
│   └── back-to-top.tsx      # Back to top button
├── lib/
│   ├── portfolio-data.ts    # All portfolio content data
│   └── utils.ts             # Utility functions
├── public/                  # Static assets
└── package.json
```

## Color System

The design uses a carefully curated color palette with semantic design tokens:

- **Primary**: Hot Pink (#ff1493) - Primary brand color
- **Secondary**: Cyan (#00d4ff) - Secondary accent
- **Accent**: Neon Green (#00ff88) - Tertiary accent
- **Warm**: Orange (#ffa502) & Magenta (#ff6b9d) - Warm accents
- **Cool**: Purple (#9d4edd) - Cool accent
- **Background**: Dark Navy (#0a0e27) - Primary background
- **Text**: Light Blue-White (#f0f4ff) - Primary text

All colors are defined in `globals.css` under CSS custom properties for easy customization.

## Getting Started

### Prerequisites
- Node.js 18+ 
- pnpm (or npm/yarn)

### Installation

1. **Clone or Download the project**
```bash
cd portfolio
```

2. **Install dependencies**
```bash
pnpm install
```

3. **Run development server**
```bash
pnpm dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser.

### Build for Production

```bash
pnpm run build
pnpm start
```

## Customization

### Update Portfolio Content
Edit `/lib/portfolio-data.ts` to customize:
- Personal information
- Work experience
- Education & certifications
- Projects
- Skills
- Social media links

### Change Colors
Edit `/app/globals.css` and update the CSS custom properties in the `.dark` selector:
```css
.dark {
  --primary: #your-color;
  --secondary: #your-color;
  /* ... more colors */
}
```

### Modify Animations
- **Duration & timing** in component files (e.g., `components/sections/hero.tsx`)
- **Global animations** in `app/globals.css` under `@keyframes`
- **Individual element animations** using Framer Motion `motion` components

### Update Fonts
Edit `app/layout.tsx` to import different Google Fonts, then update the `@theme` in `globals.css`.

## Performance Optimizations

- **Next.js 16 Turbopack**: Ultra-fast builds and Hot Module Replacement
- **Code Splitting**: Automatic route-based code splitting
- **Image Optimization**: Built-in image optimization with next/image
- **Lazy Loading**: Scroll-triggered animations with intersection observer
- **CSS-Based Animations**: Efficient animations using CSS and Framer Motion GPU acceleration

## Deployment

### Deploy to Vercel (Recommended)

1. Push your code to GitHub
2. Go to [vercel.com](https://vercel.com)
3. Import your repository
4. Vercel auto-detects Next.js configuration
5. Deploy with a single click

Environment variables are automatically handled by Vercel.

### Deploy to Other Platforms

The project uses standard Next.js App Router, so it can deploy to:
- **Netlify** - with `@netlify/plugin-nextjs`
- **AWS Amplify** - native Next.js support
- **Self-hosted** - `pnpm run build` then run with Node.js

## Browser Support

- Chrome/Edge: Latest versions
- Firefox: Latest versions
- Safari: Latest versions
- Mobile browsers: All modern versions

## Features Explained

### Staggered Animations
Components animate in sequence using Framer Motion's `variants` and `transition` props with staggered `delay` values.

### Scroll Progress Bar
A fixed-position bar at the top shows scroll progress using window scroll events and Framer Motion's `useScroll`.

### Floating Background
Four gradient orbs animate continuously in the background using Framer Motion's `animate` with infinite `repeat` transitions.

### Glassmorphism
Uses Tailwind CSS `backdrop-blur` with semi-transparent backgrounds and subtle borders to create the frosted glass effect.

### Responsive Design
Built mobile-first with Tailwind's responsive prefixes (`md:`, `lg:`, etc.) for perfect display on all screen sizes.

## Lighthouse Performance

Target metrics:
- **Performance**: 95+
- **Accessibility**: 95+
- **Best Practices**: 95+
- **SEO**: 100

## License

This portfolio template is free to use and modify for personal or professional purposes.

## Support & Questions

For questions or issues:
1. Check the code comments in component files
2. Review Framer Motion docs: [motion.dev](https://motion.dev)
3. Review Next.js docs: [nextjs.org](https://nextjs.org)
4. Review Tailwind docs: [tailwindcss.com](https://tailwindcss.com)

## Credits

Built with:
- Next.js 16
- React 19
- Tailwind CSS 4
- Framer Motion
- Lucide React Icons

---

**Ready to customize?** Start by editing `/lib/portfolio-data.ts` with your own information!
