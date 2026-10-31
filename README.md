# 🍽️ Restro

Restro is a responsive, single-page restaurant website showcasing a premium dining experience. It brings together restaurant branding, signature dishes, guest testimonials, opening hours, FAQs, and calls to action in one polished landing page.

## 🌐 Live Demo

Visit the deployed website:

<a href="https://restro-five-lake.vercel.app/" target="_blank" rel="noopener noreferrer">
  🚀 Open Restro Website
</a>

## ✨ Features

- Responsive navigation with desktop links and a mobile menu
- Hero banner and restaurant introduction
- Restaurant highlights and signature dish cards with prices
- Feature highlights for chef-crafted food, fresh ingredients, and hospitality
- An illustrated, three-step table reservation overview
- Weekly opening hours
- Guest testimonials and a collapsible FAQ section
- Repeated booking calls to action and a multi-column footer
- Scroll-triggered entrance animations and smooth scrolling

> **Reservation note:** The booking section describes the reservation process, but this project does not currently include a reservation form, booking API, or confirmation workflow. The booking buttons navigate to that section.

## 🧰 Technology

- **React 19** — component-based UI, rendered into the page from `src/main.jsx`
- **JavaScript and JSX** — application source; the project does not currently use TypeScript
- **Vite 8** — development server and production build tooling
- **Tailwind CSS 4** — utility-first styling, integrated through `@tailwindcss/vite`
- **Motion** (`motion/react`) — scroll-triggered entrance and dish hover animations
- **Lenis** — smooth scrolling
- **Lucide React** — interface icons
- **Google Fonts** — Geist and Urbanist, imported from Google Fonts in the global stylesheet

There is no backend or database configured. Restaurant content is stored in `src/data/data.jsx`; most visual assets are served from `public/assets/`. Testimonial portraits are loaded from Unsplash.

## 🚀 Getting started

### 📋 Requirements

- Node.js compatible with the installed Vite version
- npm

### 📦 Install dependencies

```bash
npm install
```

### 💻 Start the development server

```bash
npm run dev
```

Vite prints the local URL in the terminal after the server starts.

### 🏗️ Build for production

```bash
npm run build
```

The generated site is written to `dist/`.

### 🔍 Preview the production build

```bash
npm run preview
```

### ✅ Lint the project

```bash
npm run lint
```

## 🗂️ Project structure

```text
.
├── index.html                 # HTML entry point and page metadata
├── public/
│   └── assets/                # Restaurant imagery, logos, and icons
├── src/
│   ├── App.jsx                # Composes the single-page site sections
│   ├── main.jsx               # React application entry point
│   ├── index.css              # Tailwind import, fonts, and global styles
│   ├── components/
│   │   ├── Animated.jsx       # Shared scroll-reveal animation wrapper
│   │   ├── Footer.jsx         # Contact details and footer navigation
│   │   ├── LenisScroll.jsx    # Lenis smooth-scroll lifecycle
│   │   └── Navbar.jsx         # Responsive navigation
│   ├── data/
│   │   └── data.jsx           # Menu, section, FAQ, and testimonial content
│   └── sections/
│       ├── About.jsx
│       ├── BookingProcess.jsx
│       ├── CTAs.jsx
│       ├── Dishes.jsx
│       ├── FAQs.jsx
│       ├── Features.jsx
│       ├── HeroSection.jsx
│       ├── Stats.jsx
│       ├── TestimonialSection.jsx
│       └── Timing.jsx
├── vite.config.js             # React and Tailwind Vite plugins
└── package.json               # Dependencies and npm scripts
```

## 🎨 Content and customization

- Edit menu items, prices, hours, FAQs, testimonials, feature copy, and navigation links in `src/data/data.jsx`.
- Update section layout and content presentation in the corresponding component under `src/sections/`.
- Replace the restaurant images and branding in `public/assets/`. The site references these files by their `/assets/...` URLs.
- Adjust shared colors, fonts, and global styling in `src/index.css`; most component-level layout and responsive styles use Tailwind utility classes.
- Update the document title and favicon in `index.html`.

Some footer links, social links, map links, and contact details are sample or placeholder values and should be replaced with the restaurant's real information before publishing. The displayed opening hours and menu prices are also sample site content.

## 👨‍💻 Author

**Karthick Kannan R.**

Senior Web Developer | Node.js | Express.js | Next.js | React.js | Laravel

🔗 GitHub: [Karthick-kannan-24](https://github.com/Karthick-kannan-24){:target="_blank"}

🔗 LinkedIn: [Karthick Kannan R.](https://www.linkedin.com/in/Karthick-kannan-2421997/){:target="_blank"}

## 📄 License

This project was developed as part of a technical assessment.
