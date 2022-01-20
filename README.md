# Frontend Mentor - Order Summary Card Solution

This is a solution to the [Order summary card challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/order-summary-component-QlPmajDUj). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 


## Contents

  - [Screenshot](#screenshot)
  - [Built With](#built-with)
  - [What I learned](#what-i-learned)
  - [Things to Work On Going Forward](#things-to-work-on-going-forward)
  - [Useful Resources](#useful-resources)
  - [Author](#author)


### Screenshot

(images/my-desktop-view-screenshot.png)


### Built With

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid


### What I learned

- First used hidden overflow on the parent card to contain the image at the top rounded corners, 
- Because I wanted it to scroll when shrunken vertically, instead set the vertical overflow to auto
- Added the same border radius to the image as the parent card (which might make it more difficult to edit the border radius in the future)
```css
 /* overflow: hidden; */
  overflow-y: auto; 
```

- Added a box shadow to replace the default outline focus state
- "Proceed to Payment" button already had a box shadow, so the focus state didn't show when only using the universal selector
- Added a separate focus state for that button to increase the specificity and override the existing box shadow when in focus.
```css
.next-screen:focus {
  box-shadow: 0 0 0 0.7rem rgba(104, 2, 151, 0.5);
}
```

- Form elements do not inherit font from the body, so I applied the button font directly to the buttons themselves.
```css
button {
  font-family: "Red Hat Display", sans-serif;
}
```


### Things to Work On Going Forward

- Still need more practice with layout/ positioning, but this was a great exercise to help solidify the position/ flexbox/ grid concepts.
- Also need to learn more about accessibility, re font sizing, contrast, etc.
- Still struggling with responsiveness, trying to keep the design looking consistent on various screens.
- In the HTML, I need to work on cleaner, more consistent class name structures.
- I'm sure this CSS is more repetitive and clunky than it needs to be, so I need to learn more about refactoring to keep it dry.


### Useful Resources

- I've been working on a few different Udemy courses, but the most helpful so far for this particular type of challenge is from Jonas Schmedtmann: 
(https://www.udemy.com/course/design-and-develop-a-killer-website-with-html5-and-css3/) 
- Of course I also reference MDN docs a lot: (https://developer.mozilla.org/en-US/docs/Web/CSS)


### Author

- Katie
- Frontend Mentor - [@KatieB4](https://www.frontendmentor.io/profile/KatieB4)
