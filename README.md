# Frontend Mentor - Space tourism website solution

This is a solution to the [Space tourism website challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/space-tourism-multipage-website-gRWj1URZ3). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)


## Overview

### The challenge

Users should be able to:

- View the optimal layout for each of the website's pages depending on their device's screen size
- See hover states for all interactive elements on the page
- View each page and be able to toggle between the tabs to see new information

### Screenshot

![git@github.com:chelrochester/space-tourism-image.git](https://github.com/chelrochester/space-tourism-image/blob/main/space-tourism-homepage.png?raw=true)

### Links

- Live Site URL: [space tourism](https://main--inquisitive-capybara-23439a.netlify.app/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Responsive design
- Vanilla JS

  

### What I learned

- Hamburger navigation button on mobile view only

### Code

#### CSS Styling

    .sidebar {
    position: fixed;
    top: 0;
    right: 0;
    width: 250px;
    height: 100vh;
    z-index: 999;
    background-color: rgba(255, 255, 255, .1);  
    backdrop-filter: blur(5px);
    box-shadow: -10px 0 10px rgba(0, 0, 0, 0.1);
    display: none;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
}

.sidebar li {
    width: 100%;
}

.sidebar a {
    width: 100%;
}

@media only screen and (max-width: 800px) {
    .menu-icon {
        display: block;
        margin: 5px;
    }

    .hideOnMobile {
        display: none;
    }

    .navlink {
        background-color: rgba(0, 0, 0, 0);
        margin: 0;
        padding: 10px;
        height: 30px;
        width: 10px;
        display: flex;
        justify-content: flex-start;
        align-items: flex-end;
    }

    .navlink>li {
        padding: 0;
    }

    .sidebar>li {
        margin: 20px;
    }

...

#### Vanilla Javascript 

  function showSidebar(){
            const sidebar = document.querySelector('.sidebar');
            sidebar.style.display = 'flex';
        }

  function hideSidebar(){
            const sidebar = document.querySelector('.sidebar');
            sidebar.style.display = 'none';
        }

### Useful resources

- W3 Schools - I used this resource to refresh my memory on certain CSS stylings, such as removing the default styling for <a> tags.
- stack overflow - I used this when researching different solutions to problems that came up with my styling.
- MDN Web Docs - I used this to help make sure I was implementing responsive design for smaller screens correctly.

## Author

- Website - [Chesley Rochester](https://www.chelrochester.com)
- Frontend Mentor - [@chelrochester](https://www.frontendmentor.io/profile/yourusername)
- Twitter - [@chelsey8006]

