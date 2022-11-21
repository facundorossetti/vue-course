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
1) Add a method to increase the value of "count" by 1 by clicking the button and on enter key is pressed, also render the count value.

2) Watch the "count" value and change the value of count2 to: (count new value * 10).

3) Create a computed property to render the name + surname in a p tag element.

4) Create a form, bind the values of the inputs using v-model, use .lazy and .number modifiers and render the values. Also render the type value for age (it should be a number). when the button type submit is pressed, it should prevent default values on inputs (using .prevent on the event).

5) When the component is mounted print in console the value of "printMeInConsole". Get the classname of the current element using $el and render it. Also select the text of the button ref="myButton" and render it. 

6) Create a filter to capitalize the value of any string element.


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





<!-- ANSWERS
<template>
  <div id="app" class="anyClass">
    <button ref="myButton" @click="increaseCount" @keyup.enter="increaseCount">
      Increase Count + 1
    </button>
    <p>Count: {{ count }}</p>
    <p>{{ fullName }}</p>
    <p>Count2: {{ count2 }}</p>
    <p>The button text is: {{ buttonText }}</p>
    <p>The class of this app is: {{ className }}</p>
    <div class="form-container">
      <form action="submit">
        <h1>This is a form:</h1>
        <input type="text" v-model.lazy="nacionality">
        <p>Nacionality: {{ nacionality | capitalize }}</p>
        <input v-model.number="age">
        <p>Age value: {{ age }}</p>
        <p>Age type: {{ age ? typeof age : '' }}</p>
        <button type="submit" @click.prevent  >Submit</button>
      </form>
    </div>
  </div>
</template>

<script>
export default {
  name: 'App',
  filters: {
    capitalize(value) {
      if (!value) return ''
      value = value.toString()
      return value.charAt(0).toUpperCase() + value.slice(1)
    },
  },
  data() {
    return {
      name: 'John',
      surname: 'Digweed',
      count: 0,
      count2: 0,
      buttonText: null,
      printMeInConsole: 'Print this text in console when mount.',
      className: null,
      nacionality: null,
      age: null,
    };
  },
  mounted() {
    this.buttonText = this.$refs.myButton.innerHTML;
    this.className = this.$el.className;
    console.log(this.$data.printMeInConsole);
  },
  methods: {
    increaseCount() {
      this.count += 1;
    },
  },
  computed: {
    fullName() {
      return this.name + '' + this.surname;
    },
  },
  watch: {
    count(newValue, /* oldValue */ ) {
      this.count2 = newValue * 10;
    },
  },
}
</script> 
-->