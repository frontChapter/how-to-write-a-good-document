# Styling Guide

## Overview

This project uses [Tailwind CSS](https://tailwindcss.com/) for styling, integrated with the [Vite](https://vitejs.dev/) build tool. This guide explains how to customize the theme fonts and colors in a Tailwind CSS project set up with Vite. Tailwind CSS allows for easy theme customization through the `tailwind.config.js` file.

## Customizing Fonts

### Adding Custom Fonts

1. **Install the desired fonts** (if using Google Fonts, add the link to your `index.html`):

   ```html
   <!-- Add to the <head> section of index.html -->
   <link
     href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap"
     rel="stylesheet"
   />
   ```

2. **Update `tailwind.config.js`** to include the custom fonts:

   ```javascript
   module.exports = {
     theme: {
       extend: {
         fontFamily: {
           sans: ['Roboto', 'sans-serif'],
           // Add more font families as needed
         },
       },
     },
     plugins: [],
   }
   ```

3. **Apply the custom fonts** in your CSS or HTML:
   ```html
   <div class="font-sans">This text uses the Roboto font.</div>
   ```

### Changing Default Fonts

To change the default fonts, modify the `fontFamily` key in the `theme` section of `tailwind.config.js`:

```javascript
module.exports = {
  theme: {
    fontFamily: {
      sans: ['Roboto', 'sans-serif'],
      serif: ['Georgia', 'serif'],
      mono: ['Menlo', 'monospace'],
    },
  },
  plugins: [],
}
```

### Customizing Colors

Update `tailwind.config.js` to include custom colors:

```ts
module.exports = {
  theme: {
    extend: {
      colors: {
        primary: '#1E40AF',
        secondary: '#64748B',
        accent: '#F97316',
        // Add more custom colors as needed
      },
    },
  },
  plugins: [],
}
```

Apply the custom colors in your CSS or HTML:

```html
<div className="bg-primary text-white">
  This div has a custom primary background color.
</div>
<button className="bg-accent text-white">Accent Button</button>
```

---

[Go back to Readme](../README.md)
