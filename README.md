# Frontend Mentor - QR code component solution

This is a solution to the [QR code component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/qr-code-component-iux_sIO_H). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

## Overview

### Screenshot

![Screenshot of solution](images\Screenshot-of-solution.png)

### Links

- Solution URL: https://github.com/KalliKalla/qr-code-component-main
- Live Site URL: https://kallikalla.github.io/qr-code-component-main/

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox for centering
- Google Fonts (Outfit)
- Fixed-width card design

### What I learned

This project helped me understand how to properly center elements using Flexbox. I learned that the parent container needs a defined height (like `min-height: 100vh`) for vertical centering to work properly:

```css
body {
  display: flex;
  min-height: 100vh;
  justify-content: center;
  align-items: center;
}
```

I also learned about font weight standards and how to properly import  
Google Fonts:

<link href="https://fonts.googleapis.com/css2?family=Outfit:wght@400;7     
00&display=swap" rel="stylesheet">

### Continued development

In future projects, I want to focus on:

- Learning more about responsive design and when to use media queries
- Exploring CSS Grid for more complex layouts
- Improving my workflow with CSS preprocessors like Sass
- Better understanding of accessibility best practices

### Useful resources

- https://fonts.google.com - Helped me understand how to properly
  import and use web fonts
- https://css-tricks.com/snippets/css/a-guide-to-flexbox/ - This is an  
  excellent reference for Flexbox properties
- https://developer.mozilla.org - Great for understanding CSS
  properties and HTML elements

## Author

- Frontend Mentor: https://www.frontendmentor.io/profile/KalliKalla
- GitHub: https://github.com/KalliKalla
