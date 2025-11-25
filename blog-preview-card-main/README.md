# Frontend Mentor - Blog preview card solution

This is a solution to the [Blog preview card challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/blog-preview-card-ckPaj01IcS). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

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

![Screenshot of solution](assets/images/Screenshot.png)

### Links

- Solution URL: https://github.com/KalliKalla/FrontendMentor/tree/master/blog-preview-card-main
- Live Site URL: https://kallikalla.github.io/FrontendMentor/blog-preview-card-main/index.html

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Responsive design to address both mobile and desktop without media queries
- BEM naming methodology
- Self hosted font

### What I learned

I used clamp in order to make the font scale between viewport sizes. Also usesd pre-defined spacing, based on em, in order to make the spacing change with the font size.

To see how you can add code snippets, see below:

```css
.blog-preview-card__author-name {
  font-size: var(--text-size-3);
  font-weight: var(--font-weight-bold);
  margin-inline-start: var(--spacing-150);
}
```

### Continued development

In future projects, I want to focus on:

- Learning more about responsive design and when to use media queries
- Improving my workflow with CSS preprocessors like Sass
- Better understanding of accessibility best practices

### Useful resources

- [Can I Use](https://caniuse.com/) - "Can I use" provides up-to-date browser support tables for support of front-end web technologies on desktop and mobile web browsers.
- [Clamp Calculator](https://www.marcbacon.com/tools/clamp-calculator/) - There are a lot of these calculators availbale online. Good for calculating the values to use in your clamp function.

## Author

- Frontend Mentor: https://www.frontendmentor.io/profile/KalliKalla

## Acknowledgments
