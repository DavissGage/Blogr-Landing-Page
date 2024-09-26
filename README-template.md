# Frontend Mentor - Blogr landing page solution

This is a solution to the [Blogr landing page challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/blogr-landing-page-EX2RLAApP). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the site depending on their device's screen size
- See hover states for all interactive elements on the page

### Screenshot

![](./screenshot.jpg)

Add a screenshot of your solution. The easiest way to do this is to use Firefox to view your project, right-click the page and select "Take a Screenshot". You can choose either a full-height screenshot or a cropped one based on how long the page is. If it's very long, it might be best to crop it.

Alternatively, you can use a tool like [FireShot](https://getfireshot.com/) to take the screenshot. FireShot has a free option, so you don't need to purchase it. 

Then crop/optimize/edit your image however you like, add it to your project, and update the file path in the image above.

**Note: Delete this note and the paragraphs above when you add your screenshot. If you prefer not to add a screenshot, feel free to remove this entire section.**

### Links

- Solution URL: https://stackoverflow.com/questions/79004654/is-there-a-way-i-can-reuse-a-toggle-function-for-a-list-of-navigation-items-that/79004668?noredirect=1#comment139306327_79004668
- Live Site URL: https://davissgage.github.io/Blogr-landing-page/

## My process

I started with the mobile first approach. and went from there. the styling was pretty easy using a mixture of css grid and flex. 

### Built with
HTML5
CSS3
Vanilla Javascript


### What I learned

I am getting the hang of manipulating the DOM using Javascript and this is a snippet of how I created the functionality of the navigation menus. 
And closing the menu when the screen size is changed so it doesnt break when someone is changing screen sizes and forgets to close the mobile nav.
```js
const getDropDownMenus = document.querySelectorAll('#dropdown-menu')
let dropdown = document.querySelectorAll('.drop-item');



document.querySelectorAll("li.dropdown").forEach(li => li.addEventListener("click", openMenu));



function openMenu(){
    this.querySelector('.dropdown-menu').classList.toggle('active');
    this.querySelector('img.arrow').classList.toggle('active');
};


const mediaQuery = window.matchMedia('(min-width:768px)');


mediaQuery.addEventListener('change', () => {
    mobileMenu.style.display = 'none';
    hamburger.style.display = 'block';
    closeMenu.style.display = 'none';
})
```

### Continued development

I would like to learn how I can make cleaner javascript using jquery on a similar project in the future. 
I also think it wouldve been good to use SASS with a project like this to create cleaner CSS. 


## Acknowledgments

Barmar from stack overflow helped me with the functionality of the mobile navigation. 

Link to the solution:
https://stackoverflow.com/questions/79004654/is-there-a-way-i-can-reuse-a-toggle-function-for-a-list-of-navigation-items-that/79004668?noredirect=1#comment139306327_79004668
