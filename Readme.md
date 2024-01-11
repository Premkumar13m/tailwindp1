npm init -y
npm install -D tailwindcss
npx tailwindcss init -p
npm i autoprefixer
"scripts": {
    "test": "echo \"Error: no test specified\" && exit 1",
    "start": "vite"   //add in package.json file
  }
>create main.css file and add some line in this file  
@tailwind base;
@tailwind components;
@tailwind utilities;

>in tailwind.config.js add star in content

/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ["*"],     // add here star in double quotes.
  theme: {
    extend: {},
  },
  plugins: [],
}

>link the main.css in the index.html file in the heading section.

 <link href="main.css" rel="stylesheet">

 > now run the tailwindcss by writing the command i.e., npm start.
