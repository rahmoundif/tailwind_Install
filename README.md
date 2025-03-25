# tailwind_Install
Tailwind installation 2025

commmand to update output.css file : npm run build:css

1- Clone this repo.
2- install 
(if you want to do it without cloning then follow)
2- npm inity -y (so you get the package.json file)
3- npm install -D tailwindcss postcss autoprefixer (installing tailwind Postcss autoprefixer),
4- npx tailwindcss init -p 
(if this doesn't work creat manually "tailwind.config.js" and "post.config.css") :


tailwind.config.js : 

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

and postcss.config.js 

module.exports = {
  plugins: {
    tailwindcss: {},
    autoprefixer: {},
  },
}

5-create a folder named src and add a css file named : styles.css 

@tailwind base;
@tailwind components;
@tailwind utilities;

it should then work.
Cheers !
