# Frontend Mentor - Huddle landing page with single introductory section solution

This is a solution to the [Huddle landing page with single introductory section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/huddle-landing-page-with-a-single-introductory-section-B_2Wvxgi0). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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

- View the optimal layout for the page depending on their device's screen size
- See hover states for all interactive elements on the page

### Screenshot

![desktop view design image](./design/desktop-design.jpg)
![mobile view design challenge](./design/mobile-design.jpg)

![](./images/complete-project.png)

### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Flexbox
- Mobile-first workflow

### What I learned

When I looked at the design, I thought through what it is I need to accomplish with the layout at both mobile and desktop. I originally thought
that I could only apply padding to the main wrapper and things would be just fine, but the mobile view was a bit off. So I opted for using display
flex. This allowed me to add in the necessary padding at the larger screen size. 

see code snippets, below:

```html
<div class="main-content__materialBox">
  <div class="hero box"><img class="hero-img" src="./images/illustration-mockups.svg" alt="illustations"></div>
  <div class="main-content__materialBox-hookline box">
    <p class="header">Build The Community Your Fans Will Love</p>
    <p class="content">
      Huddle re-imagines the way we build communities. You have a voice, but so does your audience.
      Create connections with your users as you engage in genuine discussion.
    </p>
    <div class="content btn">Register</div>
  </div> 
</div>
```
```css
:root {
    --Mobile: 375px;
    --Desktop: 1440px;

    --Violet: hsl(257, 40%, 49%);
    --SoftMagenta: hsl(300, 69%, 71%);
    --White: #FFF;
    --attribution:hsl(228, 45%, 44%);

    --ff-Heading: 'Poppins', sans-serif;
    --ff-Body: 'Open Sans', sans-serif;

    --fw-400: 400;
    --fw-600: 600;

    --fs-header-mobile: 1.5rem;
    --fs-content-mobile: 0.75rem;
    --fs-header-desktop: 3rem;
    --fs-content-desktop: 1.25rem;

    --btn-padding-mobile: 1rem 2rem;
    --btn-padding-desktop: 1.5rem;
    --btn-width-mobile: calc(100% - 3.5rem);
    --btn-width-desktop: calc(50% - 1rem);

    --icons-social-dimensions: 1.5rem;
    --icons-social-dimensions-mobile: 1rem;

    --icon-margin-mobile: 1rem;
    --icon-margin-desktop: 1.5rem;
}
.wrapper {
    display: flex;
    flex-direction: column;
    justify-content: center;
}

.wrapper, .main-content__materialBox-hookline {
    padding: 3rem 1rem;
}

.main-content {
    flex: 1;
}

.absolute {
    position: absolute;
    top: 0;
    left: 0;
    z-index: -1;
    height: 100%;
}
```


### Continued development

I struggled a bit with managing the size of the illustration-mockup.svg image. This made transitioning from smaller screens to larger screens difficult. I am still
not sure how well I handled the background image with respect to how the design intended for it to look at different screens sizes. Overall, I am proud of what I was
able to accomplish today. 

Moving forward, continue with critically thinking about the best approach for the design. Keep practicing my flex and grid skills as well as improve my general css
knowledge.

### Useful resources

- [Example resource 1](https://www.example.com) - This helped me for XYZ reason. I really liked this pattern and will use it going forward.
- [Example resource 2](https://www.example.com) - This is an amazing article which helped me finally understand XYZ. I'd recommend it to anyone still learning this concept.

**Note: Delete this note and replace the list above with resources that helped you during the challenge. These could come in handy for anyone viewing your solution or for yourself when you look back on this project in the future.**

## Author

- Website - [Add your name here](https://www.your-site.com)
- Frontend Mentor - [@yourusername](https://www.frontendmentor.io/profile/yourusername)
- Twitter - [@yourusername](https://www.twitter.com/yourusername)

**Note: Delete this note and add/remove/edit lines above based on what links you'd like to share.**

## Acknowledgments

This is where you can give a hat tip to anyone who helped you out on this project. Perhaps you worked in a team or got some inspiration from someone else's solution. This is the perfect place to give them some credit.

**Note: Delete this note and edit this section's content as necessary. If you completed this challenge by yourself, feel free to delete this section entirely.**
