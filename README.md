# Frontend Mentor - Profile card component solution

This is a solution to the [Profile card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/profile-card-component-cfArpWshJ). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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

- Build out the project to the designs provided.

### Links

- Solution URL: [Code](https://github.com/Ivuska/frontendmentor-profile-card-component.git)
- Live Site URL: [My solution LIVE](https://ivuska.github.io/frontendmentor-profile-card-component/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow

### What I learned

#### My learning notes

**background with more image items/layers**
Background with images was a quite big challenge for me. After many attempts for the solution I ended with this piece of code and positioning the body element *relative* that hopefully solve this design task.

Quite useful knowledge could be also working with *background* property, that is not used in the project at last, but seems to be quite useful for some other tasks.

**HTML**
```
div class="bubbleWrap">
    <img src="images/bg-pattern-top.svg" class="backgroundBubbleOne" alt="" aria-hidden="true">
    <img src="images/bg-pattern-bottom.svg" class="backgroundBubbleTwo" alt="" aria-hidden="true">
  </div>
```

**CSS**
```
.bubbleWrap {
  width: 100%;
  height: 100%;
  position: absolute;
  overflow: hidden;
}

.backgroundBubbleOne {
  position: absolute;
  left: 50%;
  top: 50%;
  transform: translate(-100%, -90%);
}

.backgroundBubbleTwo {
  position: absolute;
  right: 50%;
  bottom: 50%;
  transform: translate(100%, 100%);
}
```

**positioning of the profile photo 'onto' two divs**
- I discovered that I can use margin also in a negative way :-D And that is probably more useful to add padding to the whole container
than to each different element in the container.

### Continued development
I need to train and get myself more experienced in work with background images in layers to be able to code more complicated designs combining more items together. 

I also need to improve my assesing the solution in the more contextual way:
- see the component as a part of the bigger complex so maybe using the h1 element can cause some problems when adding the component to the more complex solution.
- do not forget that using of ul/li elements with proper CSS styling can be more comfrotable for screenreaders than to use the h2 and p 
elements 

### Useful resources

- [Transform property MDN documentation](https://developer.mozilla.org/en-US/docs/Web/CSS/transform) - in the simplified way - this property "draws" the element on some place on the screen where I need it while the element iself has the unchaged position. 
- [Overflow property MDN documentation](https://developer.mozilla.org/en-US/docs/Web/CSS/overflow) 
- [Background property MDN documentation](https://developer.mozilla.org/en-US/docs/Web/CSS/background) 

## Author

- Frontend Mentor - [@Ivuska](https://www.frontendmentor.io/profile/Ivuska)
