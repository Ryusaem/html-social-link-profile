# Frontend Mentor - Social links profile solution

This is a solution to the [Social links profile challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/social-links-profile-UG32l9m6dQ). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

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

## Overview

### The challenge

Users should be able to:

- See hover and focus states for all interactive elements on the page

### Screenshot

![Screenshot Project](/design/screenshot-project-ryusaem.png)

### Links

- Solution URL: [GitHub](https://github.com/Ryusaem/html-social-link-profile)
- Live Site URL: [Github Live Demo](https://ryusaem.github.io/html-social-link-profile/)

## My process

- Using Version Control: Utilize Git for version control. Make regular commits to track changes and manage versions. This is helpful for undoing changes and understanding the evolution of your project.
- Responsive Design: Implement responsive design practices to ensure that your social link profile looks good on all devices.
- Choose a Hosting Platform: Deploy your project on a reliable web hosting platform like GitHub Pages, Vercel, Netlify, or a similar service.

- Create HTML Structure:

  - The boilerplate has been made by Frontend Mentor.
  - Head Section: In the <head>, link your CSS files, add a title with <title>, and include any meta tags needed for responsiveness (<meta name="viewport" content="width=device-width, initial-scale=1.0">).
  - Body Content: In the <body>, lay out your content using semantic HTML:

    - Header: Use <header> for profile image and name.
    - Main Section: Use <main> for bio and social links. Each social link can be an <a> tag inside a <div> or <section>.
    - Footer: Use <footer> for copyright information and additional links.

  - Set Up a CSS File:

    - Link a CSS file in the <head> section of your HTML using <link rel="stylesheet" href="styles.css">.
    - Reset style:

    ```css
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }
    ```

    - Layout Styling: Use Flexbox or Grid to layout your sections. For example, to center content and layout vertically:

    ```css
    body {
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      min-height: 100vh;
    }
    ```

    - Responsive Design: Use media queries to adjust styles on different screen sizes. For example:

    ```css
    @media (max-width: 768px) {
      .container {
        max-width: 90vw;
      }
    }
    ```

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow

### What I learned

- To use an image as an Avatar, you have to convert the image into a perfect square, otherwise the image will look like a weird losange.

- To push some "footer" and other "div" at the bottom of the screen, use the "margin-top: auto". I work very well in a flexbox environment.

```css
.attribution {
  margin-top: auto; /*Ensures it sticks to the bottom*/
}
```

- Learn in a better way how to use "transition" and "transform" property in CSS, which can add pretty cool effect on your code. But let's be honest, I need much more practice and understanding on how animation work, I'm still a pure novice.

```css
.button {
  transition: transform 0.3s ease, background-color 0.3s ease;
}

.button:active,
.button:hover {
  transform: scale(1.1); /* Slightly scale down the button when pressed */
}
```

- Learn to use the "custom css variable" a little bit more, which is very powerful to make all the change we want in only one line of code. What a powerful concept.

```css
:root {
  /* --primary-color: #1f1f1f; */
  --primary-color: hsl(0, 0%, 12%);
  --secondary-color: hsl(75, 94%, 57%);
  --background-color: hsl(0, 0%, 8%);
  --gray-color: hsl(0, 0%, 20%);
  --white-color: hsl(0, 0%, 100%);
}
```

- I also learn more how to control responsive element to make a better code in either mobile and desktop view. Modifying the width (especially the max-width) is an important process to make the website look beautiful. We could also add some margin in the mobile view to add more style.

```css
.container {
  max-width: 30vw;
}

@media screen and (max-width: 768px) {
    .container {
        margin-top: 30px;  /*Adjusts the margin-top for smaller screens*/
        max-width: 95vw;  /*Adjusts the width for smaller screens*/
    }
```

- Learn that using the attribute "rel="noopener noreferrer" is a good measure to prevent security risk. That also remind me on how to open a page in a new page 'target="\_blank" '. I also learn that using attribute 'aria-label' is a good way to allow people that use screen reader to know when you are referencing to a link.

```html
<a
  href="https://github.com/Ryusaem"
  class="button"
  aria-label="Visit GitHub profile"
  target="_blank"
  rel="noopener noreferrer"
>
  GitHub
</a>
```

### Continued development

- Animation in CSS.
- Flexbox (the power of using margin inside any flex item).
- Responsivity (Media query understanding).
- Knowing how much a project is going to take as time.
- Learning to deconstruct a website in a Flexbox way to be much more efficient.

### Useful resources

- [Frontend Mentor](https://www.frontendmentor.io/challenges/recipe-page-KiTsR8QQKm) - Formidable resources to make you learn by "doing" awesome project. Highly recommend it.
- [Square an Image](https://squareanimage.com/) - This help me to square my avatar to a perfect Square.

## Author

- Github - [@Ryusaem](https://github.com/Ryusaem)
- Linkedin - [@sambath-meas](https://www.linkedin.com/in/sambath-meas)
- Coursera - [@sambath-meas](https://www.coursera.org/learner/sambath-meas)
- Twitter - [@RyuBraveheart](https://twitter.com/RyuBraveheart)
- Frontend Mentor - [@Ryusaem](https://www.frontendmentor.io/profile/Ryusaem)
- CodeWars - [@Ryusaem](https://www.codewars.com/users/Ryusaem)
