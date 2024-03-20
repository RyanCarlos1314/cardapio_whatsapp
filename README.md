# cardapio_whatsapp
 Software de cardapio com integração ao Whatsapp

# 1-Install Tailwind CSS
Install tailwindcss via npm, and create your tailwind.config.js file.

Execute no Terminal

npm install -D tailwindcss

npx tailwindcss init

# 2-Configure your template paths
Add the paths to all of your template files in your tailwind.config.js file.

configure na pasta -> tailwind.config.js

/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ["./src/**/*.{html,js}"],
  theme: {
    extend: {},
  },
  plugins: [],
}

# 3-Add the Tailwind directives to your CSS
Add the @tailwind directives for each of Tailwind’s layers to your main CSS file.

adicione dentro da sua pasta de estilos -> src/input.css

@tailwind base;
@tailwind components;
@tailwind utilities;

# 4-Start using Tailwind in your HTML
Add your compiled CSS file to the <head> and start using Tailwind’s utility classes to style your content.

<!doctype html>
<html>
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <link href="./output.css" rel="stylesheet">
</head>
<body>
  <h1 class="text-3xl font-bold underline">
    Hello world!
  </h1>
</body>
</html>


# 5-command to run tailwind
npm run dev
