# reset.css

A lightweight, minimal & modern reset.css to provide a consistent baseline for styling across different browsers.

## What Does the Reset Do?

### 1. Universal Box Sizing

```
*,
*::before,
*::after {
  box-sizing: border-box;
}
```

> Ensures that padding and borders are included in the element's total width and height.

### 2. Remove Default Margin

```
*,
html,
body {
  margin: 0;
  padding: 0;
}
```

> Removes the default margins and paddings from all elements.

### 3. Smooth Scrolling & Text Adjustments

```
html {
  scroll-behavior: smooth;
  -moz-text-size-adjust: none;
  -webkit-text-size-adjust: none;
  text-size-adjust: none;
}
```

> Enables smooth scrolling and disables browser-specific text size adjustments.

### 4. Base Body Styles

```
body {
  line-height: 1.5;
  -webkit-font-smoothing: antialiased;
}
```

> Sets the default line height for the body and applies antialiased font smoothing.

### 5. Media Elements

```
img,
picture,
video,
canvas,
svg {
  display: block;
  max-width: 100%;
  font-style: italic;
}
```

> Ensures that media elements are displayed as block-level elements and scale within their containers.

### 6. Form Styles

```
input,
button,
textarea,
select {
  font: inherit;
  word-spacing: inherit;
  letter-spacing: inherit;
}
```

> Makes sure that form elements inherit their font and spacing properties from their parent elements.

### 7. Link and List Styling

```
a {
  color: inherit;
  text-decoration: none;
}
ul,
li,
ol {
  list-style: none;
}
```

> Removes the default link color and underline and resets the list styles.

### 8. Typography

```
p,
h1,
h2,
h3,
h4,
h5,
h6 {
  overflow-wrap: break-word;
}
h1,
h2,
h3 {
  text-wrap: balance;
  line-height: 1.2;
}
p {
  text-wrap: pretty;
}
```

> Ensures text elements wrap properly and headings have a balanced line height.

### 9. Reduced Motion Support

```
@media (prefers-reduced-motion: reduce) {
  html {
    scroll-behavior: auto;
  }
  * {
    animation-duration: 0.01ms !important;
    animation-iteration-count: 1 !important;
    transition-duration: 0.01ms !important;
    scroll-behavior: auto !important;
    transition: none;
  }
}
```
> Detects if a user prefers reduced motion and minimizes animations and transitions.
