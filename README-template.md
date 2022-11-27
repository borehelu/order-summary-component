# Frontend Mentor - Order summary card solution

This is a solution to the [Order summary card challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/order-summary-component-QlPmajDUj). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Useful resources](#useful-resources)
- [Author](#author)




## Overview

### The challenge

Users should be able to:

- See hover states for interactive elements

### Screenshot

![](./screenshot.png)


### Links

- Solution URL: [github link](https://github.com/borehelu/order-summary-component)
- Live Site URL: [live link](https://your-live-site-url.com)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Preprocessor SASS
- Mobile-first workflow




### What I learned

I learnt the importance of using preprocessors to speed up the writing of css styles following the DRY philosophy. SASS allowed to use the typical programming constructs in CSS making the entire process very enjoyable. I enjoyed using mixins to encapsulate reusable styles under a name that I could include everywhere the group of styles were needed.




```scss
@mixin flex{
    display: flex;
    justify-content: center;
    align-items: center;
    
}
```

```scss
.btn{
    padding: .9rem;
    border:none;
    width: 100%;
    font-weight: 700;
    border-radius: 8px;
    cursor: pointer;
    transition: all .3s ease-out;
}

```

```scss
     & .primary{
            @extend .btn;
            background-color: $bright-blue;
            color: $white;
            box-shadow: 0 10px 15px rgba($color: $bright-blue, $alpha: 0.3);
            

            &:hover{
                background-color: desaturate($color: $bright-blue, $amount: 25%);
            }
        }
```






### Useful resources

- [w3schools Sass Tutorial](https://www.w3schools.com/sass/default.php) - This helped me get quickly upto speed with the syntax for SASS.




## Author


- Frontend Mentor - [@borehelu](https://www.frontendmentor.io/profile/borehelu)
- Twitter - [@helu_bore](https://www.twitter.com/helu_bore)



