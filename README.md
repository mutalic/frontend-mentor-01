## Table of contents

- [Screenshot](#screenshot)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
- [Author](#author)

### Screenshot

Mobile version: ./screenshots/mobile.png
Desktop version: ./screenshots/desktop.png


## My process

1. HTML architecture.
2. Reset some default CSS behavior (box-sizing, <body> margin, <html> font-family & font-size).
3. Styled elements in the order of: .container -> qr-code box -> text

### Built with

- CSS custom properties (variables)
- Flexbox
- Mobile-first workflow

**Note: These are just examples. Delete this note and replace the list above with your own choices**

### What I learned

1. Removing whitespace below <img> elements.
  - <img> elements are inline by default, so I changed the display to 'block' to remove whitespace.
  ```css
  .qr-img {
    width: 100%;
    height: 100%;
    display: block; /* Removes whitespace below image. */
  }
  ```
2. Applying border-radius to images.
  - First set border-radius, then set overflow to 'hidden'.
  ```css
  .qr-img-box {
    border-radius: 15px;
    overflow: hidden;
    padding: 0;
  }
  ```
3. Vertically center <div> on screen.
  - Set <body> height to 100vh.
  - Give <body> display of 'flex'.
  - <body> has justify-content: center and align-items: center.
  ```css
  body {
    height: 100vh;
    margin: 0;
    display: flex;
    justify-content: center;
    align-items: center;

    background-color: var(--main-bg-color);
  }
  ```

### Continued development

1. Need structured system for naming CSS classes.
2. Start out with creating classes for fonts and colors before styling anything else.

## Author

- Website - [Jason Hwang](https://github.com/mutalic)
- Frontend Mentor - [@mutalic](https://www.frontendmentor.io/profile/mutalic)
