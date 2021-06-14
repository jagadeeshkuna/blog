<template>
  <div id="blog">
<h3>New Blog </h3>
<form>
  <label>Blog Title:</label>
  <input type="text" v-model.lazy="blog.title" required/>
  <label>Content inside the Blog</label>
  <textarea v-model.lazy="blog.content"></textarea>
</form>
<div id="preview">
  <h3>Blog preview</h3>
  <p>Blog Title: {{blog.title}}</p>
  <p>Content in the Blog: {{blog.content}}</p>
  </div>
  </div>
</template>

<script>

export default {

  data(){
    return{
      blog:{
      title: "",
      content: ""
      }

    }
  }
}
</script>
<style>
body{
  margin: 0;
  font-family:Arial Narrow;
}
</style>
