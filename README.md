# tailwind_Install
Tailwind installation 2025

commmand to update output.css file : npm run build:css

1- Clone this repo.
<br>
2- npm install tailwindcss to get the node_modules to use for it.

(if you want to do it without cloning then follow)
<br>
1- npm inity -y (so you get the package.json file)
<br>
2- npm install -D tailwindcss postcss autoprefixer (installing tailwind Postcss autoprefixer),
<br>
3- npx tailwindcss init -p 
<br>
(if this doesn't work creat manually "tailwind.config.js" and "post.config.css") :
<br>
<br>


tailwind.config.js : 
<br>

/** @type {import('tailwindcss').Config} */
module.exports = {
  content: [
    "./src/**/*.{html,js,jsx,ts,tsx}", // Adjust this based on your project structure
    "./index.html"
  ],
  theme: {
    extend: {},
  },
  plugins: [],
}

<br>
<br>
and postcss.config.js 
<br>

module.exports = {
  plugins: {
    tailwindcss: {},
    autoprefixer: {},
  },
}
<br>
<br>
5-create a folder named src and add a css file named : styles.css 
<br>
@tailwind base;
@tailwind components;
@tailwind utilities;
<br>
<br>
it should then work.
Cheers !
