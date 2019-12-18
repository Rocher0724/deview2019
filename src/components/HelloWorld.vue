<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <h3>링크</h3>
    <ul>
      <li><a href="https://github.com/" target="_blank"                         >normal link</a></li>
      <li><a href="https://github.com/" target="_blank" rel="whale-sidebar"     >whale side bar link</a></li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  method: {
    newWindow() {
      window.open()
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
