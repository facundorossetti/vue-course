<template>
  <div id="app" class="anyClass">
    <button ref="myButton">
      Increase Count + 1
    </button>
    <p>Count: {{  }}</p>
    <p>Full name: {{  }}</p>
    <p>Count2: {{  }}</p>
    <p>The button text is: {{  }}</p>
    <p>The class of this app is: {{  }}</p>
    <div class="form-container">
      <form action="submit">
        <h1>This is a form:</h1>
        <input type="text" placeholder="nacionality">
        <p>Nacionality: {{  }}</p>
        <input placeholder="age">
        <p>Age value: {{  }}</p>
        <p>Age type: {{  }}</p>
        <button type="submit">Submit</button>
      </form>
    </div>
  </div>
</template>


<script>
export default {
  name: 'App',
  filters: {},
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
  mounted() {},
  methods: {},
  computed: {},
  watch: {},
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
.form-container form {
  display: flex;
  align-items: center;
  flex-direction: column;
  gap: 15px;
}
.form-container form input {
  max-width: 200px;
}
</style>

