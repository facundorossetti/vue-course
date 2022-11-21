# hello-world

## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Lints and fixes files
```
npm run lint
```

### TASKS:

<!--
1) Render the "exampleText" value into a h1 tag inside the div with id "app".
2) Add a class called "red-text" to the element id "redParagraph" and any inline-style.
3) Bind the style of the element id "redParagraph" with "exampleStyle".
4) Add conditional rendering v-if to the element with id "conditionalRendered". It only will render if "exampleBoolean" is true, but if it's false the element with id "conditionalRendered2" should be rendered.
5) Create an iteration of the array "exampleArray" using v-for and render inside a p tag containing the "name" value of each element and concat the sume of (5 + "id") value using javascript expressions.

*********** NOTE: YOU CAN FIND THE ANSWERS AT THE END OF THE FILE. ***************
-->





-
-
-
-
-
-
-
-





<!-- SOLUTIONS
<template>
  <div id="app">
    <p>{{ exampleText }}</p>
    <p class="red-text" style="border: 2px solid blue" :style="exampleStyle" id="redParagraph">I want to be a Red text.</p>
    <p v-if="exampleBoolean === true" id="conditionalRendered">I want to be rendered if "exampleBoolean" is true.</p>
    <p v-else id="conditionalRendered2">I want to be rendered if "exampleBoolean" is false.</p>
    <p id="styleBinded">Bind me a style.</p>
    <div v-for="(element, index) in exampleArray" :key="index" id="iterated">
      <p>{{ element.name }} {{ 5 + element.id }}</p>
    </div>
  </div>
</template> -->