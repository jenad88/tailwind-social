# tailwind-social
Tailwind example project learned from Dr Sahand Ghavidel's course

npm install -D tailwindcss
npm install -D @tailwindcss/forms

npx tailwindcss init

tailwind.config.js:
module.exports = {
  content: ["./src/**/*.{html,js}"],
  theme: {
    extend: {},
  },
  plugins: [
    require('@tailwindcss/forms),
  ],
}

src/input.css:
@tailwind base;
@tailwind components;
@tailwind utilities;

npx tailwindcss -i ./src/input.css -o ./dist/output.css --watch
