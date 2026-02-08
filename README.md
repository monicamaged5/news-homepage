# Frontend Mentor - News Homepage Solution

This is my solution to the [News Homepage Challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/news-homepage-H6SWTa1MFl). This challenge helped me improve my frontend skills by building a realistic, responsive project.

## Table of Contents

* [Overview](#overview)

  * [The Challenge](#the-challenge)
  * [Screenshot](#screenshot)
  * [Links](#links)
* [My Process](#my-process)

  * [Built With](#built-with)
  * [What I Learned](#what-i-learned)
  * [Continued Development](#continued-development)
  * [Useful Resources](#useful-resources)
* [Author](#author)
* [Acknowledgments](#acknowledgments)

## Overview

### The Challenge

Users should be able to:

* View the optimal layout for the interface depending on their device's screen size
* See hover and focus states for all interactive elements on the page

### Screenshot

![alt text](<Desktop preview.png>)
![alt text](<Mobile preview.png>)

### Links

* Solution URL: [https://github.com/monicamaged5/news-homepage]
* Live Site URL: [https://monicamaged5.github.io/news-homepage/]

## My Process

### Built With

* Semantic HTML5 markup
* CSS custom properties
* Flexbox & CSS Grid
* JavaScript

### What I Learned

During this project, I focused on responsive design. Some highlights:

```html
<ul>
    <li><img src="assets/images/logo.svg" alt="logo"></li>
    <li><a class="hideOnMobile" href="#">Home</a></li>
    <li><a class="hideOnMobile" href="#">New</a></li>
    <li><a class="hideOnMobile" href="#">Popular</a></li>
    <li><a class="hideOnMobile" href="#">Trending</a></li>
    <li><a class="hideOnMobile" href="#">Categories</a></li>
    <li><img class="menu-button" onclick="showSidebar()" src="assets/images/icon-menu.svg" alt="menu-icon"></li>
  </ul>```

```css
@media (max-width: 790px ){
   .hideOnMobile{
      display: none;
   }
   .menu-button{
      display:block;
   }
   body{
       padding: 1rem;
   }
   .container{
    grid-template-columns: 1fr !important;
   }
   .leftside{
   width: 100%;

   }
}
```

```js

    function hideSidebar(){
      const sidebar = document.querySelector('.sidebar');
      sidebar.style.display='none';
    };
```

### Continued Development

In future projects, I want to:

* Improve accessibility and ARIA roles
* Optimize responsive typography and spacing
* Explore animations and interactive UI elements

### Useful Resources

* [MDN Flexbox Guide](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Flexbox) – Helped me understand layout patterns
* [CSS Tricks Grid Guide](https://css-tricks.com/snippets/css/complete-guide-grid/) – Essential for building responsive grids

## Author

- Frontend Mentor - [@monicamaged5](https://www.frontendmentor.io/profile/monicamaged5)

## Acknowledgments

Thanks to Frontend Mentor for providing this challenge and to the community for inspiration and feedback.

