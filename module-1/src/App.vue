<template>
  <div id="app">
    <p id="redParagraph">I want to be a Red text.</p>
    <p id="conditionalRendered">I want to be rendered if "exampleBoolean" is true.</p>
    <p id="conditionalRendered2">I want to be rendered if "exampleBoolean" is false.</p>
    <p id="styleBinded">Bind me a style.</p>
    <div id="iterated">
      <p></p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'App',
  data() {
    return {
      exampleText: 'Hi, I am an example text.',
      exampleText2: 'I am another example text.',
      exampleBoolean: false,
      exampleBoolean2: true,
      exampleStyle: 'background-color: lightblue',
      exampleArray: [
        {
          id: 1,
          name: 'first element',
        },
        {
          id: 2,
          name: 'second element',
        },
        {
          id: 3,
          name: 'third element',
        },
      ],
    };
  },
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
.red-text {
  color: red;
}
</style>
