# Frontend Mentor - QR code component solution

This is a solution to the [QR code component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/qr-code-component-iux_sIO_H).

## Table of contents

- [Overview](#overview)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
- [Author](#author)

## Overview

### Screenshot

![Screen shot of QR project](https://github.com/willetto/Frontend-Mentor-1/blob/main/QR%20Screen%20Shot.png?raw=true)

### Links

- Solution URL: [CSS File](https://github.com/willetto/Frontend-Mentor-QR/blob/main/style.css)
- Live Site URL: [Github Pages](https://willetto.github.io/Frontend-Mentor-QR/)

## My process

### Built with
- Visual Studio Code
- Semantic HTML5 markup
- CSS custom properties
- Flexbox

### What I learned

The original reference image had the faintest shadow around the entire component, and my first attempts at replicating it were too bold. I finally tried putting a negative value for the spread-radius. In effect, this shrunk the shadow evenly underneath the container, leaving only the lightest, most-feathered part of the box-shadow remaining.

```css
.container {
box-shadow: 0 0 20px -10px var(--grayishBlue);
}
```
I also wanted to center both the QR component and the attribution both vertically and horizontally on the page. Using auto margin was able to center it horizontally, but not vertically. I wrapped the both my container and attribution into a div with a class of "super-container" using flex to center all of the contents vertically.

```css
.super-container {
  position: relative;
  height: 100vh;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}
```

### Continued development

I want to find a neater, cleaner solution to centering componets onto a page. I also had to guess at the border-radius values. I want to figure out either the math or a better method for matching those curves.

## Author

- Website - [Trey Willetto](https://www.treywilletto.com)
- Frontend Mentor - [@willetto](https://www.frontendmentor.io/profile/willetto)
