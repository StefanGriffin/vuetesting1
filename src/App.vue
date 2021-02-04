<template>

<img alt="" src="">
<div> {{ greet }} {{ name }}</div>
<div v-html="channel"></div>
<div v-html="hack"></div>
<h2 v-bind:id="HeadingId">Heading</h2>
<button v-bind:disabled="isDisabled">Click Me</button>
<h2 class="underline">Underline text</h2>
<h2 v-bind:class="status">Status</h2>
<h2 v-bind:class="isPromoted && 'promoted'">Promoted Movie</h2>
<h2 v-bind:class="isSoldout ? 'sold-out': 'new'">Sold-out ? movie</h2>

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
      status: 'succes',
      isPromoted: true,
      isSoldout: true,
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

.underline {
  text-decoration: underline;
}


.promoted{

font-style: italic;

}

.new {
  color: rgb(103, 26, 122);
}

.sold-out {
  color:rgb(135, 166, 201);
}

</style>
