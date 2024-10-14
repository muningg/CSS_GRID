# CSS Grid Example Project

This project shows how to use CSS Grid for making responsive layouts. It has several pages that show different ways to use Grid.

## Why is this important?

CSS Grid helps create complex, two-dimensional layouts. It's great for making designs that look good on different screen sizes and devices.

## What's included?

1. A main page with navigation
2. Employee cards page
3. Student profiles page
4. Delivery information page
5. Examinee information page

## Key CSS Snippets

### Basic Setup

```css
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    display: grid;
    grid-template-rows: auto 1fr;
    background-color: #f0f0f0;
}
```

This sets up the basic grid layout for the whole site.

### Grid Navigation

```css
.nav-container {
    display: grid;
    place-items: center;
    height: calc(100vh - 100px);
}

.nav-list {
    list-style: none;
    padding: 0;
    display: grid;
    gap: 15px;
}
```

This makes a centered grid layout for the navigation menu.

### Card Layout

```css
.employee-container,
.student-container,
.delivery-container,
.examinee-container {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    gap: 20px;
    padding: 20px;
}
```

This creates a responsive grid layout for cards that adjusts based on screen size.

### Hover Effects

```css
.employee-card:hover,
.student-card:hover,
.delivery-card:hover,
.examinee-card:hover {
    transform: translateY(-5px);
}
```

This makes cards move up a little when you hover over them.

## How to Use

1. Open `index.html` in your browser to see the main page.
2. Click on the links to see different pages.
3. Make your browser window bigger or smaller to see how the layout changes.

Feel free to change the CSS to try out different Grid properties!

## Key Differences from Flexbox

- Grid works in two directions (rows and columns) at the same time.
- The `grid-template-columns` property with `repeat(auto-fit, minmax(200px, 1fr))` makes a layout that changes the number of columns automatically.
- `place-items: center` is an easy way to center things in grid layouts.

Try both Flexbox and Grid to see which one works better for your layouts!

---

To see a similar project using CSS Flexbox instead of Grid, check out:
[muningg/CSS_FLEX](https://github.com/muningg/CSS_FLEX)
