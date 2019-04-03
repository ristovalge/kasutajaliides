<template>
  <div class="card">
    <header class="card-header">
      <p class="card-header-title">
        {{post.title}}
      </p>


    </header>
    <div class="card-content">
      <div class="content">
{{post.content}}

      </div>
    </div>
    <footer class="card-footer">
      <a href="#" class="card-footer-item">Save</a>
      <a href="#" class="card-footer-item">Edit</a>
      <a href="#" class="card-footer-item">Delete</a>
    </footer>
  </div>
</template>

<script>
    export default {
        name: "Post",
      props: ['post']
    }
</script>

<style scoped>

</style>
