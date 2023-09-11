# Frontend Mentor - NFT preview card component solution

This is a solution to the [NFT preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/nft-preview-card-component-SbdUL_w0U). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Useful resources](#useful-resources)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover states for interactive elements

### Screenshot

## Desktop Preview

![](./screenshot.jpg)

## Desktop Preview States

![](./screenshot.jpg)

## Mobile Preview

![](./screenshot.jpg)

## Mobile Preview States

![](./screenshot.jpg)

### Links

- Solution URL: [Solution](https://your-solution-url.com)
- Live Site URL: [NFT Preview Card](https://your-live-site-url.com)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- FlexBox
- CSS Grid
- Mobile-first workflow
- StyleLint

### What I learned

The major thing I did on this project is to fix the image hover wherein a view icon will appear popup or overlay after pointing the cursor to the nft image.

```html
<div class="card-image">
  <img
    src="./images/image-equilibrium.jpg"
    alt="an equilibrium with transparent feel and look"
    class="nft-image"
  />
  <img
    src="./images/icon-view.svg"
    alt="eye shape for image view"
    class="view-image"
  />
</div>
```

```css
#parent .card .card-image {
  position: relative;
  width: 100%;
  height: 100%;
}

#parent .card .card-image img.nft-image {
  width: 100%;
}

#parent .card .card-image .view-image {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  opacity: 0;
}

#parent .card .card-image:hover,
#parent .card .card-image:hover .view-image {
  opacity: 1;
  cursor: pointer;
}
```

### Useful resources

- [ChatGPT](https://www.example.com) - This helped me for finding answers to my questions. I really liked this pattern and will use it going forward.

## Author

- Website - [Shanice Cleofe](https://github.com/sdacleofe/about-me)
- Frontend Mentor - [@sdacleofe](https://www.frontendmentor.io/profile/sdacleofe)
