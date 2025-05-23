# Frontend Mentor - Meet landing page solution

This is a solution to the [Meet landing page challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/meet-landing-page-rbTDS6OUR). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover states for interactive elements

### Links

- Solution URL: [solution URL](https://github.com/Patrycja-dz/fm-meet-landing-page-)
- Live Site URL: [ live site URL](https://patrycja-dz.github.io/fm-meet-landing-page-/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties (variables) for theming and reusability
- Flexbox for layout (e.g., navigation, footer content)
- CSS Grid for image gallery layout
- Mobile-first workflow, with responsive design for tablet and desktop
- CSS animations and transitions for hover effects and page load elements

### What I learned

This project was a great opportunity to practice building a responsive landing page from scratch. Some key takeaways include:

- **CSS Custom Properties for Theming:** Leveraging CSS custom properties (variables) extensively, made it easy to manage colors, fonts, and spacing consistently. For example:

  ```css
  :root {
    --color-cyan-600: #4d96a9;
    --font-family-heading: "Red Hat Display", sans-serif;
    --space-4: 1rem;
  }

  .hero__title {
    color: var(--color-slate-900);
    font-family: var(--font-family-heading);
    margin-block: var(--space-4);
  }
  ```

- **Responsive Images and Layouts**: Implementing different background images and layout adjustments for mobile, tablet, and desktop views using media queries. The hero section and footer backgrounds change based on screen size, and the image grid adjusts its columns.

```css
.hero__image {
  background-image: url("../assets/tablet/image-hero.png");
}

.grid {
  grid-template-columns: repeat(2, 1fr);
}

@media (min-width: 90em) {
  .hero__image {
    background-image: none;
  }
  .grid {
    grid-template-columns: repeat(4, 1fr);
  }
  .footer {
    background-image: url("../assets/desktop/image-footer.jpg");
  }
}
```
