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

<header class="nav-header">
        <nav class="nav">
            <img src="\starter-code\assets\shared\logo.svg" alt="icon" id="logo">
            <ul class="navlink barlow-condensed-regular">
                <li class="hideOnMobile"><a href="/home.html">00 Home</a></li>
                <li class="hideOnMobile"><a href="/destination.html"> 01 Destination</a></li>
                <li class="hideOnMobile"><a href="/crew.html">02 Crew</a></li>
                <li class="hideOnMobile"><a href="/technology.html">03 Technology</a></li>
                <li class="menu-icon" id="menu-icon" onclick=showSidebar()><a href="#" ><svg xmlns="http://www.w3.org/2000/svg" width="24" height="21"><g fill="#D0D6F9" fill-rule="evenodd"><path d="M0 0h24v3H0zM0 9h24v3H0zM0 18h24v3H0z"/></g></svg></a></li>
            </ul>
            <ul class="sidebar barlow-condensed-regular">
                <li onclick=hideSidebar()><a href="#"><svg xmlns="http://www.w3.org/2000/svg" width="20" height="21"><g fill="#D0D6F9" fill-rule="evenodd"><path d="M2.575.954l16.97 16.97-2.12 2.122L.455 3.076z"/><path d="M.454 17.925L17.424.955l2.122 2.12-16.97 16.97z"/></g></svg></a></li>
                <li><a href="/home.html">00 Home</a></li>
                <li><a href="/destination.html"> 01 Destination</a></li>
                <li><a href="/crew.html">02 Crew</a></li>
                <li><a href="/technology.html">03 Technology</a></li>
            </ul>
        </nav>
    </header>

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


### Useful resources

- W3 Schools - I used this resource to refresh my memory on certain CSS stylings, such as removing the default styling for <a> tags.
- stack overflow - I used this when researching different solutions to problems that came up with my styling.
- MDN Web Docs - I used this to help make sure I was implementing responsive design for smaller screens correctly.

## Author

- Website - [Chesley Rochester](https://www.chelrochester.com)
- Frontend Mentor - [@chelrochester](https://www.frontendmentor.io/profile/yourusername)
- Twitter - [@chelsey8006]

