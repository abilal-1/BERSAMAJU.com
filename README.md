# BERSAMAJU.com — Astro Website

A modern, responsive, and accessible landing page for **BERSAMAJU**, built with **Astro** and **Tailwind CSS v4**.

---

## ⚠️ If you see `'npm' is not recognized` in your terminal

Node.js is installed at `C:\Program Files\nodejs\`. Your existing terminal window was opened before Node was installed and hasn't loaded the new `PATH` yet.

### Quick Fix (Choose one):
1. **Option A (Easiest)**: Close your current terminal tab in VS Code / IDE (`Ctrl + ~` or the trash icon on the terminal) and **open a new terminal** (`Ctrl + Shift + \`` or `Terminal -> New Terminal`).
2. **Option B (Instant in current PowerShell)**: Run this one line in your terminal:
   ```powershell
   $env:Path = [System.Environment]::GetEnvironmentVariable("Path","Machine") + ";" + [System.Environment]::GetEnvironmentVariable("Path","User")
   ```

After that, `npm` and `node` will work immediately.

---

## 🚀 Getting Started

> **Note:** The project is already created and fully configured! You **do not** need to run `npm create astro`.

### Run Development Server
```sh
npm run dev
```
Open [http://localhost:4321](http://localhost:4321) in your browser.

### Production Build
```sh
npm run build
```
The optimized production output is generated in `./dist/`.

### Preview Production Build
```sh
npm run preview
```

---

## 📁 Project Structure

```text
/
├── public/                 # Static assets
├── src/
│   ├── components/         # Astro UI components
│   │   ├── Navbar.astro
│   │   ├── MobileMenu.astro
│   │   ├── HeroSection.astro
│   │   ├── AboutSection.astro
│   │   ├── ProgramSection.astro
│   │   ├── TestimonialSection.astro
│   │   ├── BlogSection.astro
│   │   ├── CTASection.astro
│   │   ├── Footer.astro
│   │   ├── AccessibilityWidget.astro
│   │   └── AuthModal.astro
│   ├── layouts/
│   │   └── Layout.astro    # Base HTML layout with SEO & dark mode script
│   ├── pages/
│   │   └── index.astro     # Landing page
│   └── styles/
│       └── global.css      # Tailwind v4 theme & accessibility styles
├── package.json
└── astro.config.mjs
```

---

## ✨ Features

- **Component Architecture**: 11 modular, reusable `.astro` components
- **Tailwind CSS v4**: Powered by `@tailwindcss/vite` with custom theme tokens
- **Dark Mode**: Toggle button with localStorage persistence and FOUC prevention
- **Interactive Modals & Menus**: Mobile slide-out drawer, Auth login/signup modal
- **Accessibility Tools**: Floating widget with font sizing, contrast adjustments, and reduced motion
- **SEO & Performance**: Zero client JS overhead for static sections, instant load times
