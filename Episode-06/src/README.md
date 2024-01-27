# Episode 4 [ Let's get Hooked ]
 
 * HEADER
 * - Logo
 * - Navbar
 *  - Home
 *  - About
 *  - Cart
 * BODY
 * - Search
 * - RestaurantCard
 *   - Img
 *   - Name of Restaurant, cuisine, Rating, delivery time
 * FOOTER
 * - Copyright
 * - links
 * - Address


Two types of Export/ Import


- default Export/Import
export default component;
import component from "path";

- Named Export/Import
export const component;
import {component} from "path";

Onclick event takes a callback function
- ```js
   <button onclick={ () => {
    console.log("Button clicked");
    }}></button>


`Note` : JS is very fast in DOM manipulation, that's why JS is fast


# React Hooks

- Hooks are just normal JS utility functions

useState( ) : Generate superpowerful react variable in react
- it keeps the UI in sink with the variable.
- whenever a state variable update, react re-renders its component

useEffect( ): 

#### Reconcialiation Algorithm
- React uses reconcialiation (whenever something chnages on UI, known as reconcialiation) algo. (also known as React Fiber).

- let's say restaurant container has a 7 res-card, on clicking the button, it filters and update to 3 res-card

#### Virtual DOM
- it is a representation of Actual DOM

```HTML
Actual DOM
<div>
    <div>
        <img>
    </div>    
</div>
```

Virtual DOM is just a Normal JS Object

### Diff Algorithm
- it finds difference b/w updated virtual DOM and previous DOM, then, actually updates the DOM on every render cycle.

- like the ex. of Reconcialiation Algo.
- As soon as clicked on the button, a new object is formed and React find the difference b/w prev obj and the new obj like there was 7 res-card and now, it's 3 res-card, then it actually updates the DOM

###### Why React is fast?
- It is fast and efficient at DOM Manipulation
- It has a diff Algo, which is very efficient.

## [React Fiber documentaion](https://github.com/acdlite/react-fiber-architecture)



