# React-installing-solution
For install the new website with React javascript

React.js
A. Installation
1. > npm init vite
- Project name: <project name (kebab case)>
- framework: >> react
- variant: >> react

2. > cd <project name>
3. > npm install

B. Setup#1
4. delete file - .gitignore, package-lock.json, src/logo.svg, src/index.css
5. Re-write: src/App.css clear all
6. Delete line: import './index.css' in file src/main.jsx
7. Re-write: src/App.jsx clear all and then
Edit: 
import React from 'react';

export default function App() {
  return <div></div>;
}
8. Re-write: vite.config.js
Edit:
import { defineConfig } from "vite";
import react from "@vitejs/plugin-react";

// https://vitejs.dev/config/
export default defineConfig({
  plugins: [react()],
  server: {
    port: 3005,
  },
});


C. Setup#2 Install packages
> npm install react-bootstrap bootstrap@5.1.3
> npm install --save @fortawesome/fontawesome-free
> npm install -S axios sweetalert2
> npm instal -S react-router-dom