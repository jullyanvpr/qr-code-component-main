# README.md

# Frontend Mentor - QR code component solution

This is a solution to the [QR code component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/qr-code-component-iux_sIO_H). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Table of contents](#table-of-contents)
- [Overview](#overview)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
- [Author](#author)
- [Acknowledgments](#acknowledgments)


## Overview

### Screenshot

![Printscreen from the application](./images/printscreen.png)

### Links

- Solution URL: [https://github.com/jullyanvpr/qr-code-component-main](https://github.com/jullyanvpr/qr-code-component-main)
- Live Site URL: [https://tiny-figolla-c0f9a0.netlify.app/](https://tiny-figolla-c0f9a0.netlify.app/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox

### What I learned

It gave me a deeper understanding of how the parent-child concept works in HTML and CSS. For example, when working with images, the width rule needed to be applied directly to the child element instead of the parent:

```css
.container__qrCode__item {
    width: 100%;    
    border-radius: 15px;
}
```

Also when I applied alignment rules to the parent div containing the divs that contained img and paragraph tags, they were not being properly aligned. Instead, I had to apply separate alignment rules to their immediate parent in order to achieve the desired result.

```css
/* This served to align the divs that contained the items */
.container {
    display: flex;
    flex-direction: column;
    align-items: center;
}

/* This served to align the items themselves within the div */
.container__upper {
    display: flex;
    align-items: center;
    justify-content: center;
    padding: 10px 20px;
    text-align: center;
    font-size: 1.7rem;
    font-family: 'Outfit', sans-serif;
    font-weight: 700;
    color: var(--terciaryColor);
    
}
```

### Continued development

I would like to practice mobile-first workflow concepts and also CSS grid. I’m comfortable with using flexbox, but I haven’t used CSS grid yet.

## Author

- Github - [https://github.com/jullyanvpr](https://github.com/jullyanvpr)
- Frontend Mentor page - [https://www.frontendmentor.io/profile/jullyanvpr](https://www.frontendmentor.io/profile/jullyanvpr)

## Acknowledgments

I’d like to thank the developers community for all the free learning content and I’d like to thank frontendmentor’s staff and members.
