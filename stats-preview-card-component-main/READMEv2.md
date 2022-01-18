# Frontend Mentor - Stats preview card component solution

This is a solution to the [Stats preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/stats-preview-card-component-8JqbgoU62). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)


## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size


### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow

### What I learned

I learned alot about mixed-blend-mode and was reminded about my glaring weaknesses in responsive web design. It was a very awesome experience all in all. Here are some piece of info that I seen in stack overflow. I would like to try to explain it to prove to myself if I really grasped the solution. We adding a div to the image element with a class name of wrapper. We styled wrapper to be an inline-block with a relative position. Using the css psuedo class after we made the image an absolutely positioned element relative to itself (wrapper). It is also a block element that is rooted to the parent elements via top and bottom at 0px (0 pixels away from the top and bottom of the parent container). mixed-blend mode used since I didn't use background to add the image which added the background color to the color in the after wrapper. It was awesome!

```html
 <div class="image wrapper">
       <img class="image" src="images/image-header-desktop.jpg"/>
      </div>
```
```css
.wrapper{
        display: inline-block;
        position: relative;
      }
  
      .wrapper::after{
        content: "";
        position: absolute;
        display: block;
        top:0;
        bottom:0;
        background-color: hsl(277, 64%, 61%);
        mix-blend-mode: multiply;
        opacity: 90%;
      }
```

### Continued development

Use this section to outline areas that you want to continue focusing on in future projects. These could be concepts you're still not completely comfortable with or techniques you found useful that you want to refine and perfect.

**Note: Delete this note and the content within this section and replace with your own plans for continued development.**

### Useful resources

- [Resource 1](https://www.stackoverflow.com) - This place is like old-reliable to me. It helped me understand why certain things occurred in the front-end giving me a better understanding of my mistakes and how to approach them in the future! 
- [Resource 2](https://www.csstricks.com) - There are many amazingly relevant articles in this website so I will rely on this web site in future projects!
 

## Author

- Website - [Kheyyon](https://www.github.com/keyy123)
- Frontend Mentor - [@keyy123](https://www.frontendmentor.io/profile/keyy123)
- Linkedin - [@kheyyon-parker](https://www.linkedin.com/in/kheyyon-parker)
