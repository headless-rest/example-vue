<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <h2>Your Blog Posts</h2>
    <div v-for="(post, i) in posts" :key="i">
      <h3>{{ post.content.en.title }}</h3>
      <div v-html="post.content.en.body"></div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'hello',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App',
      posts: []
    }
  },

  created () {
    // you should do this in the VueX store
    this.posts = require('@/../headless/content/blog.json')
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1,
h2 {
  font-weight: normal;
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
