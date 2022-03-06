# Tailwind.css Tutorial

- Credit to "How to Build Unique, Beautiful Websites with Tailwind CSS" by Ivaylo Gerchev
- https://www.sitepoint.com/tailwind-unique-beautiful-websites/

## Tailwind Set-Up:
- install tailwinds with `npm install tailwindcss`
- run `npx taildwind init` to generate `tailwind.config.json`
- create base css file
    - give this file this content to import core styles from tailwind
    ```
    @tailwind base;

    @tailwind components;

    @tailwind utilities;
    ```
- now, adjust your tailwind.config.json to find your HTML file in the content. if your file is in the root of your project directory, your config.json could look like this:
```
module.exports = {
  content: ["./index.html"],
  theme: {
    extend: {},
  },
  plugins: [],
}
```

- run `npx tailwindcss -i styles.css -o output.css` to generate a tailwind stylesheet 
- link to this `output.css` in your index.html file to see tailwind styles
