<template>

<img alt="" src="">
<div> {{ greet }} {{ name }}</div>
<div v-html="channel"></div>
<div v-html="hack"></div>
<h2 v-bind:id="HeadingId">Heading</h2>
<button v-bind:disabled="isDisabled">Click Me</button>

</template>



<script>

export default {
  name: 'App',
  data() {
    return {
      greet: "Hello",
      name: "Stef Griffin 2021",
      channel: "<b>codeyourideas</b>",
      hack: `<a href="#" onclick="alert('This is a joke')">Win a prize!</a>`,
      headingID: "heading",
      isDisabled: false,
    };
  },
};
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
</style>
