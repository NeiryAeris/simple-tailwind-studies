# simple-tailwind-studies
 
# React + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

# simple step to initiate a vite, react, tailwind:
- npm create vite@latest
- chose anything
- chose react
- chose javascript
- npm install
- npm install -D tailwindcss postcss autoprefixer
- npx tailwindcss init -p

# the tailwind.config.js file at least should have this
`export default {
  content: [
    './index.html',
    './src/**/*.{js,tx,jsx,tsx}'
  ],
  theme: {
    extend: {},
  },
  plugins: [],
}
`

# the postcss.config.js file normally have this
`export default {
  plugins: {
    tailwindcss: {},
    autoprefixer: {},
  },
}
`

# the index.css file should have these inside
`@tailwind base;
@tailwind components;
@tailwind utilities;`