# Frontend Mentor - Stats preview card component solution

This is a solution to the [Stats preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/stats-preview-card-component-8JqbgoU62). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
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

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size

### Screenshot

![](./screenn-shot-desktop.png)
![](./screenn-shot-mobile.png)

### Links

- Solution URL: [Add solution URL here](https://github.com/Rod-Barbosa/Stats-preview-card-component)
- Live Site URL: [Add live site URL here](https://github.com/Rod-Barbosa/Stats-preview-card-component/blob/gh-pages/index.md)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow

### What I learned

This project was good to take the dust off of some css basics.

Most interesting for me was refactoring the way I was adding the pictures. Initially I used an img tag, but adding imageson CSS using the background-image property proved much better for dynamism and responsiveness. I learned about the differences between vh and wh units, they proved very helpfull and will certainly become a main stay on my code practices.

```html
        <div class="imagem-desktop">
            <!-- <img src='image-header-desktop.jpeg' alt="beautiful people in the office"></img> -->
        </div>
        <div class="imagem-mobile">

        <!-- <img src='image-header-mobile.jpg' alt="beautiful people in the office"></img> -->
        </div>
```
```css
.imagem-desktop{
    background-image: url('image-header-desktop.jpeg');

}
.imagem-mobile{
    background-image: url('image-header-mobile.jpg');
    background-size: cover;
    height: 30vh;
    border-top-left-radius: 10px;
    border-top-right-radius: 10px;
    min-width: 100%;
}
```

Using media query was also interesting. Testing various screen sizes with the inspect tool from the browser proved easy once the images were being added via CSS. For some reason that scapes me, adding images via img tag made cell phone screen sizes not responsive at all

```css
@media only screen and (min-width: 1000px)  {}
```


### Continued development

There is a clear need for me to improve on @media query and background-image attachment 

### Useful resources

- [Example resource 1](https://www.w3schools.com/cssref/pr_background-image.asp) - This helped with several examples that are easy to visualize and copy. In the future hopefully I wil not need to check on W3Schools so much as things get more and more ingrained in my memory.

## Author

- Website - [Rodrigo](https://gelatodigital.com)
- Frontend Mentor - [@yourusername](https://www.frontendmentor.io/profile/yourusername)


## Acknowledgments

Thank you for my mentor Frederico Bicharra and my friend Guilherme Dias for the moral support.
