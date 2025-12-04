# React App 

// ...existing code...
# Tailwind CSS with Vite — Quick Start

This README shows the steps from the attached screenshot to set up Tailwind CSS with a Vite project (Windows PowerShell).

Prerequisites
- Node.js (16+ recommended) and npm
- Git (optional for source control)

1) Create a new Vite project
```css
npm create vite@latest "my-project name"
cd my-project
```
3) Install Tailwind CSS and the Vite plugin
```css
npm install tailwindcss @tailwindcss/vite
```
5) Configure the Vite plugin
Create or update vite.config.ts:

```ts

import { defineConfig } from 'vite'
import react from '@vitejs/plugin-react'
import tailwindcss from '@tailwindcss/vite'

export default defineConfig({
  plugins: [
    react(),       // React ke liye
    tailwindcss()  // Tailwind ke liye
  ],
})


// import { defineConfig } from 'vite'
// import tailwindcss from '@tailwindcss/vite'

// export default defineConfig({
//   plugins: [
//     tailwindcss(),
//   ],
// })
```

4) Import Tailwind in your CSS
Create a CSS file (e.g., src/style.css  OR src/index.css) and add:

```css
/* src/style.css */
/* src/index.css */
@import "tailwindcss";

:root {
  font-family: system-ui, Avenir, Helvetica, Arial, sans-serif;
  line-height: 1.5;
  font-weight: 400;

  color-scheme: light dark;
  color: rgba(255, 255, 255, 0.87);
  background-color: #242424;

  font-synthesis: none;
  text-rendering: optimizeLegibility;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

```

5) Start the dev server
```css
npm run dev
(or npm start if your package.json maps start to the dev script)
```

7) Example HTML usage
Include the compiled CSS or the dev dev server CSS in your HTML and use Tailwind classes:

```html
<!doctype html>
<html>
  <head>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width,initial-scale=1" />
    <link href="/src/style.css" rel="stylesheet" />
  </head>
  <body>
    <h1 class="text-3xl font-bold underline">Hello world</h1>
  </body>
</html>
```

Notes
- If you see "git : The term 'git' is not recognized...", install Git for Windows: https://git-scm.com/download/win
- Adjust the CSS import method to your build flow (Tailwind usually requires PostCSS; check Tailwind docs for your project type).

References
- Tailwind CSS docs: https://tailwindcss.com
- Vite docs: https://vitejs.dev
// ...existing code...


